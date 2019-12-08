# NascentCore agent

An agent accepts model for training and manages heterogenous computing devices
on a Kubernetes node. It typically owns some CPU cores and all of GPUs, and any
additional ML accelerator devices.

An agent does:

*   Compiles data flow graph into machine code that can be executed on CPU, GPU, and other type of ML accelerator chips.
*   Manages the training task, and in the case of distributed training, the pipelining of the inter-dependent training tasks on multiple nodes.
