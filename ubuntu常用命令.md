解压文件到指定位置
```
tar xvJf 下载/node-v7.4.0-linux-x64.tar.xz -C software/node2
```
创建目录并把`压缩包里面的内容`，解压到此位置，
```
mkdir software/node2 && 
tar xvJf 下载/node-v7.4.0-linux-x64.tar.xz 
-C software/node2 
--strip-components 1
```
复制文件夹里面的内容到指定的文件夹中，指定的文件夹不存在时候，自动生成
```
cp -r software/node2 software/node3
```
复制指定文件夹到当前目录
```
cp -rf software/node2 .
-f 如果目标位置存在重名的，先删除再复制进去，也就是覆盖
```
## vim
查找替换
```
:%s/old/new/g
```
