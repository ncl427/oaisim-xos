# eNodeB emulator XOS service

It is based on the vBBU XOS service for CORD 4.0
**Synchronizer code, XProto Models and Policies** are generic.

**Steps and Roles** do the configuration required for the OAISIM VNF to correctly generate multiple UE.
- The actual VNF is an image that can be downloaded in the following link [eNodeB VM Image](http://ncl.jejunu.ac.kr/M-CORD_IMAGES/files/vBBU_compress.qcow2)
- The image has the Open Air Interface eNodeB compiled on its master version. The build was generated using the parameters for creating a OAISIM environment.
- The XOS service configures the VNF with the correct IPs for the **vMME** and **vSPGW-U** connection plus general configuration requirements.

Description of this section can be found [here](xos/synchronizer/steps)

This repo is part of a *CORD 4.0* deployment, the service needs to be cloned into the `cord/orchestration/xos-services/` directory before starting XOS.
After cloning, rename the folder to **vbbu**

**To DO** Erase all the vbbu references to avoid any cause of confusion about the functionality of this service.

We plan to include a script to facilitate integration of this service with a CORD deployment.

## Acknowledgment
This research was supported by the MSIP (Ministry of Science, ICT and Future Planning), Korea, under the ITRC (Information Technology Research Center) support program (IITP-2017 2017-0-01633) supervised by the IITP (Institute for Information & communications Technology Promotion.
