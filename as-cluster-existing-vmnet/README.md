# HDInsight (Creates Linux HDI cluster with 2 head nodes 3 ZK nodes configurable workers and 1 edge nodes, requires existing Virtual Network)

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftrystanleftwich%2Fazure-quickstart-templates%2Fmaster%2Fas-cluster-existing-vmnet%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Ftrystanleftwich%2Fazure-quickstart-templates%2Fmaster%2Fas-cluster-existing-vmnet%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>


Builds a Linux HDI cluster, configurable version, head, worker and edge node size and number of workers.
Requires existing Virtual Network.

This will create a 2 Head node, 3 Zookeeper, N worker nodes and 1 edge node Linux HDI cluster based on the version you provide (tested on 3.4)
It will use the provided Virtual Network for all IPs and all new servers will be put into the subnet of you provide.
It will create a new Public IP and Load balancer for the Edge node and both Head Nodes in the clusters resource group.
It will create a new Storage account in the clusters resource group.
