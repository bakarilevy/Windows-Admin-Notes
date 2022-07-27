To create disk partitions from the command line you must run a terminal window as an administrator:

```
diskpart
```

You will see a prompt that looks like this:

```
DISKPART>
```

First list the disks available:
```
list disk
```

To select a disk enter:
```
select disk <#>
```

To create a new partition enter the following:

```
create partition size=<512>
```

You will then be prompted with the type of partition you would like to create if you are using a disk that is using the Master Boot Record you will create a logical disk for example:

```
create partition logical size=<512>
```

To check the available partitons on a disk enter:

```
list partition
```

We will then need to format the partiton, first lets select the partition:

```
select partition <6>
```

Then we run:
```
format fs=ntfs label=<HCL> quick
```

Now we would like to assign a letter to this partition, this can be done with the following command:

```
assign letter=<x>
```

