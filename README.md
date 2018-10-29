# eNodeB emulator XOS service

It is based on the vBBU XOS service for CORD 4.0
**Synchronizer code, XProto Models and Policies** are generic.

**Steps and Roles** do the configuration required for the OAISIM VNF to correctly generate multiple UE.
- The actual VNF is an image that can be downloaded in the following link *Not Available Yet*
- The image has the Open Air Interface eNodeB compiled on its master version. The build was generated using the parameters for creating a OAISIM environment.
- The XOS service configures the VNF with the correct IPs for the **vMME** and **vSPGW-U** connection plus general configuration requirements.

This repo is part of a *CORD 4.0* deployment, the service needs to be cloned into the `cord/orchestration/xos-services/` directory before starting XOS.
After cloning, rename the folder to **vbbu**

**To DO** Erase all the vbbu references to avoid any cause of confusion about the functionality of this service.

I plan to include a script to facilitate integration of this service with a CORD deployment.
