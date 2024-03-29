#
# Use the Global Recursive action to gather up all the source files under a variable called APP_SOURCES
#
# NOTE: Anytime you add a new .cpp files, the entire project must be cleaned and rebuilt or the new files
# will not be included in the compilation process.  This is the one drawback of GLOB_RECURSE implicit inclusion.
#
FILE(GLOB_RECURSE SOURCES src/*.cpp)
#
# Exposes components to both source and header files.
set(REQUIRES
    nvs_flash
    efuse
)
#
# Anything that must be exposed to the sources files, but may remain hidden from the header files.
# Using private requires helps to reduce possible linking error in very large applications.
set(PRIV_REQUIRES
    main
)
#
#
idf_component_register(SRCS ${SOURCES}
                       INCLUDE_DIRS "include"
                       REQUIRES ${REQUIRES}
                       PRIV_REQUIRES ${PRIV_REQUIRES}
                      )