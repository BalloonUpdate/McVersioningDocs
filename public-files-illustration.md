## public目录下的文件用途介绍

Mc Versioning在运行时会创建许多文件，本章节会主要介绍这些文件的用途，尤其是public目录下的文件

public目录下的文件一般不建议手动修改，如特殊情况确实要手动修改，请在修改之前详细阅读本章节的文件说明。如果你在使用软件的时候出现了一些不可逆转的错误，请尽量直接删除整个public目录重头来过，而非进来手动修改文件

### public/snapshot目录

这个目录用来存储client目录的最新快照。有两个用途：一是用来给客户端提供文件更新下载，二是用来丢弃你对client目录的更改的。此目录由程序自动维护，非特殊情况请勿手动修改

### public/snapshot.json文件

这个文件用来存储snapshot目录下的文件结构信息，正常情况下此文件内容应该和snapshot目录的文件结构保持一致。此外这个文件也被用来计算与client目录的差异，以此来得知你对client目录都做了哪些修改。此文件由程序自动维护，非特殊情况请勿手动修改

### public/all-versions.txt文件

这个文件存储着迄今为止你创建的所有版本号，用来给客户端判断落后服务端多少个版本。此文件由程序自动维护，非特殊情况请勿手动修改

### public/current-version.txt文件

这个文件存储着最新的版本号，用来给客户端快速判断客户端是否需要更新，如果需要更新，则客户端会再次获取all-versions.txt文件判断具体落下了哪些更新。此文件由程序自动维护，非特殊情况请勿手动修改

### v-x.x.x.json文件

x.x.x代表一个实际的版本号。这是一个版本记录文件，是存储每个版本里的文件变化的文件，也就是每个版本你都新增了哪些文件，修改了哪些文件，删除了哪些文件之类的，每一个版本都是一个单独的文件。此文件由程序自动维护，非特殊情况请勿手动修改