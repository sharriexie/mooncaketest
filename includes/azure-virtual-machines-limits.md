资源|默认限制|最大限制
---|---|---
每个云服务的[虚拟机](../articles/virtual-machines/virtual-machines-linux-azure-overview.md)数<sup>1</sup>|50|50
每个云服务的输入终结点数<sup>2</sup>|150|150

<sup>1</sup>在服务管理中创建的虚拟机会自动存储在云服务中。你可以向该云服务添加更多虚拟机以获得负载均衡和可用性。请参阅[如何将虚拟机连接到虚拟网络或云服务](../articles/virtual-machines/virtual-machines-linux-classic-connect-vms.md)。

<sup>2</sup>输入终结点允许从某个虚拟机的云服务外部与该虚拟机通信。位于同一云服务或虚拟网络中的虚拟机可以自动相互通信。请参阅[如何设置虚拟机的终结点](../articles/virtual-machines/virtual-machines-windows-classic-setup-endpoints.md)。

<!---HONumber=Mooncake_1207_2015-->