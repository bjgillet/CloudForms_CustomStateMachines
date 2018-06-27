# CloudForms Custom State Machines

A way to dynamically select VM provisioning/retirement StateMachines by tagging catalog items. 

Covers both Infrastructure and Cloud VMs. Preserves the default behavior if no explicit custom setup is done on VM catalog items, so is totally transparent to standard logics.

Some use cases are :

* Several people working at VM state machine level, needing to hav dedicated states without disturbing others.
* As services may be provisioned with pre-requisites (i.e. IPAM, CMDB,...) abitlity to still use VM Lifecycle raw provisioning.
* Specifying dedicated VM provisioning workflows based on typology while reducing complexity of huge StateMachines with lot of messages maintenance (i.e VM level Ansible Embedded workflows)
* Quick partial rollbacks without impacting all provisionings done on the platform (State Machine switching by tagging). 

Full documentation may be found at this repo wiki here : ![CustomStateMachines](https://github.com/bjgillet/CloudForms_CustomStateMachines/wiki/CustomStateMachines-Documentation)
