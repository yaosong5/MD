---
title:  
tags:  
categories: 
grammar_cjkRuby: true
---

`nohup   & `后台运行
## 文件查找
`find / -type f -size +10G`
在Linux下如何让文件让按大小单位为M,G等易读格式，S size大小排序。  `ls -lhS`
`du -h * | sort -n `  
当然您也可以结合管道文件夹内最大的几个文件  ` du -h * | sort -n|head`
动态显示机器各端口的链接情况`while :; do netstat -apn | grep ":80" | wc -l; sleep 1; done`

##sed
更改第一行 `sed -i '1s/.*//'`     sed -i '1s/.*/想更改的内容/'
删除第一行`sed -i '1d'  `     sed -i '1d' 文件名
插入第一行 `sed -i '1i\' `       sed -i ‘1i\内容‘ 文件名
## cpu
`cat /proc/cpuinfo | grep processor | wc -l`
`lscpu`
