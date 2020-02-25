# patroni_playbooks
The unbreakable, scalable elephant - playbooks 

This contains the playbooks and templates I ran during my presentation at the SwissPUG Event in Basel (20-FEB-2020).

In case you want to rerun the playbooks. You need 4 VMs for the patroni cluster (+1 for ansible):

1.  Run the playbook under "patroni" to install a 3 node patroni cluster.
2.  Run the playbook under "patroni_add" to install a 4th node and add it to the existing 3 Node Patroni cluster.
    This version does not upscale the etcd cluster.

This playbooks are not perfect. But they work ;-)

Please keep in mind that this playbooks install the DMK of dbi services as well. As this tool is only for our customers, I removed the files. You need to adjust the playbooks according to this.
