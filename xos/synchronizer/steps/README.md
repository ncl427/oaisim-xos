## Steps description

In this section there are 2 important files, a *yaml (Ansible) playbook* and a *python tenant synchronizer file*.

The **Tenant synchronizer file** contains the specific instructions for synchronizing information between the Virtual Machine and the XOS Service. One of this specific functions is the `def get_spgwu_list(self):`
This function will collect the information of all the **spgwu** instances that are being instantiated and save it as a *List* `spgwu_iplist`.

The second file related to the **Ansible Playbook** will prepare some variables for the configuration of the Virtual Machine, this variables include the IP addresses of the **vMME, eNodeB and the SPGWU List**. These will be later used on each configuration steps on the *roles* [section](roles).  
