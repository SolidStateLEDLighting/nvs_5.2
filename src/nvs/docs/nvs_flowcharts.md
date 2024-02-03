# NVS Flowcharts
___
This NVS object is a mid-level handler for storage.  This object is an extension for any other object that calls to it.

It abstracts away the lower level Esp IDF functions into a more generalized call.  We have several purposes encapsulated in these functions:

1) If NVS does not exist in FLASH, this object will establish it.
2) If any particular value does not exist, it uses the value from the caller (by ref) to set the intial value in NVS.
3) It gets all values before a set.  If those values already are the same, another set does not happen.


**NOTE:** A read always occurs at the start of all objects and it is at this point that any new variables are written into nvs with their default values:

This is the Read pattern for integers.
![NVS Write Diagram](./drawings/sntp_flowcharts_integer_read_pattern.svg)
___  
This the Write pattern for integers.
![NVS Write Diagram](./drawings/sntp_flowcharts_integer_write_pattern.svg)
___  