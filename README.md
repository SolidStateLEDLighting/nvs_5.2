# NVS 5.2 Overview
---
## Primary Objective

The NVS class is just a collection of functions which act as a mid-level abstraction between object and the calls to the IDF.

Read the abstractions here: [NVS abstraction](./src/nvs/docs/nvs_abstractions.md)

There are no block diagrams, because NVS is just a collection of functions and very little data.

Here are the flows charts for the functions: [flowcharts](./src/nvs/docs/nvs_flowcharts.md)

There are no squences because NVS has no tasks, no run loops, or no sequential processing.

We also have no state models, because NVS does not hold any states internally.  NVS has no controllable lifecycle within the project. 