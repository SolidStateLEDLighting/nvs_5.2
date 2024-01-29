# NVS 5.2 Overview

The NVS class is just a collection of functions which act as a mid-level abstraction between object and the calls to the IDF.

Read the abstractions here: [NVS abstraction](./src/nvs/docs/nvs_abstractions.md)

There are no block diagrams, because NVS is just a collection of functions and very little data.

Here are the flows charts for the functions: [flowcharts](./src/nvs/docs/nvs_flowcharts.md)

There are no squences because NVS has no tasks, no run loops, or no sequential processing.

We also have no state models, because NVS does not hold any states internally.  NVS has no controllable lifecycle within the project.

The following categories will help you visualize different aspects of NVS:

1) [NVS Abstractions](./docs/nvs_abstractions.md)
2) [NVS Block Diagram](./docs/nvs_blocks.md)
3) [NVS Flowcharts](./docs/nvs_flowcharts.md)
4) [NVS Operations](./docs/nvs_operations.md)
5) [NVS Sequences](./docs/nvs_sequences.md)
6) [NVS State Models](./docs/nvs_state_models.md)