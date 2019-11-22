# Baremetal OCP with SR-IOV and kubevirt

This repo contains the templates used for a PoC deployment of baremetal OCP
nodes with SR-IOV and kubevirt.

## SR-IOV

* Deployed sriov-network-operator to configure and deploy required pods.
* Deploy policy1.yaml and policy2.yaml to create VFs
* Deploy network-cr1.yaml and network-cr2.yaml to create SriovNetwork objects
  which inturn will create NetworkAttachmentDefinitions in the required
  namepsace mentioned as "networkNamespace"
* Create pod or vm using the NetworkAttachmentDefintions

