
## pxctl cheatsheet

**Cluster Status**

| Command | Description |
| --- | --- |
| pxctl cluster -h  | List of supported commands |
| pxctl cluster list | List nodes in the cluster, Cluster ID, Cluster UUID |
| pxctl cluster inspect <node ID> | Inspect node |

**Complete Status**

| Command | Description |
| --- | --- |
| pxctl status  | Gives a complete output/status of cluster/nodes/storagedevice/storagepool |

**Volume Management - Create**

| Command | Description |
| --- | --- |
| pxctl volume -h  | List of supported commands |
| pxctl volume create -h | List of additional commands which can be used while creating volume |
| pxctl volume create `<volname>` -s `<size default 1GB>` | Example of how to create a volume |
| pxctl volume list | List number of volumes |
| pxctl volume inspect `<VOL ID>` | Detailed information about the volume created and attached to node and disk size used |
| pxctl volume clone --name `<CloneName> <VolName>` | Clone the volume | 

**Volume Management - Update**

| Command | Description |
| --- | --- |
| pxctl volume update -h  | List of supported commands |
| pxctl volume ha-update | Update the replication factor default is 1 and max you can set is 3 |


**Volume Management - Snapshot**

| Command | Description |
| --- | --- |
| pxctl volume snapshot -h  | List of supported commands |
| pxctl volume snapshot create --name `<SnapName> <VolName>` | Snapshot the volume, Snapshots are Read-Only | 

**Service Management**

| Command | Description |
| --- | --- |
| pxctl service -h  | List of supported commands |
| pxctl service info | Prints OCI version |
| pxctl service kvdb members | List kvdb cluster members |

