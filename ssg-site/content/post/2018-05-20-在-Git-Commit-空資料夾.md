---
title: Git Commit 空資料夾
date: 2018-05-20 22:52:15
tags:
- Git
categories:
- 版本控制
description: Git Commit 空資料夾
thumbnail:
---
Git 基本只對檔案作版控，資料夾中若沒有檔案是無法 commit 的，若想要 commit 空資料夾才可採取下面兩種做法。

>新增 .gitkeep / .keep

在目的空資料夾開啟 Git Bash，執行以下命令，產生空檔案

```
$ touch .gitkeep
```

檔案名稱其實隨意都可，但 .gitkeep / .keep 較常見。

>新增 .gitingore

在目的空資夾下新增一個 .gitingore 檔案並編輯如下

```
# 忽略所有文件
*
# 除了這個文件
!.gitignore
```

我個人是比較喜歡第一種作法，讓 .gitingore 還是總控在根目錄下。