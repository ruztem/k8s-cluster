# k8s-cluster
1 master &amp; 2 worker


The first step is to prepare an Ubuntu account for convenience.

ansible-playbook -i hosts initial.yml

The second step is to prepare all the necessary components.

ansible-playbook -i hosts kube-dependencies.yml

The third step is to configure the master node and worker node.

ansible-playbook -i hosts master.yml

ansible-playbook -i hosts workers.yml
