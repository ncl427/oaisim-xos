## Roles description

This section contains the Ansible playbook instructions that are going to be applied when deploying the **OAISIM Virtual Machine (VNF)**

The **pre-requirement** section sets the Linux Host name of the machine to *oaisim* in order to easily identified in console.

The **oaisim-configure** section has the actual playbook instructions for *VM deployment* and is organized as follows:
- defaults
- tasks
- templates

**Defaults** sets up some variables with pre-determined values that refer to the **Public Land Mobile Network** description.
**Tasks** has the instructions that are going to be run as *console commands* (Like a Script) and will setup the VM with the right IPs and also the correct **Configuration File** required for it to run.
**Templates** Has the **Configuration File** necessary to run the **eNodeB Emulator** it uses variables defined in the **Defaults** section and also the variables defined in the **Steps** Playbook File for completing information related to the **PLMN** and the **MME** and **SPGWU** connections.

With this instructions the eNodeB VNF can have the correct configuration before operation.
