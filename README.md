# memmove
FPGA IP Core for moving data between modules.

### Usage

Module must be used with the **Commblock**.

```
                                                                  +---------+
                                                                  |         |
                                                            +<----+ Mod. 1  |
+-------------+    +-------------+                          |     |         |
|             |    |             |                        +------->         |
|             |    |             |   +--------------+     | |     +---------+
|             |    |             |   |              |     | |
|  Commblock  |    |   memmove   |   |              |     | |
|             |    |             |   |   Simple     +-----> |     +---------+
|             +--->+             +-->+ Interconnect |     | |     |         |
|             |    |             |   |              +<----+ +<----+ Mod. 2  |
|             |    |             |   |              |     | |     |         |
|             |    |             |   +--------------+     +------->         |
|             |    |             |                        | |     +---------+
+-------------+    +-------------+                        | |
                                                          | |          .
                                                          | |          .
                                                          | |
                                                          | |     +---------+
                                                          | |     |         |
                                                          | +<----+ Mod. N  |
                                                          |       |         |
                                                          +------->         |
                                                                  +---------+
```
