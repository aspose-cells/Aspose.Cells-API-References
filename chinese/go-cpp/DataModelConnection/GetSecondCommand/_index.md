---
title: "GetSecondCommand 方法"
linktitle: "GetSecondCommand"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetSecondCommand 方法。封装了在 Go 中表示 getsecondcommand 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/datamodelconnection/getsecondcommand/
---

## GetSecondCommand function

指定在使用 PivotTable 服务器端页面字段时持久化的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛（前者不包含 WHERE 子句）。基于这两个命令（Command 和 ServerCommand），可以填充参数 UI 并构建参数化查询。

```go

func (instance *DataModelConnection) GetSecondCommand()  (string,  error) 

```

## 备注


## 另请参阅

* Class [DataModelConnection](../)
* Library [Aspose.Cells for Go](../../)
