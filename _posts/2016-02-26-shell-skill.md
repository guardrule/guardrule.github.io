---
layout: post
title: SHELL技巧
---
### 执行技巧 ###
将待执行SHELL语句写入文件并用其它用户执行

    {
    cat << EOF
    do something ...
    EOF
    } | su - oracle | tee -a $LOG

获得当前执行目录

    currdir=`cd dirname($0) && pwd`

--EOF--
