---
title: "CellsHelper_CreateSafeSheetName_String_Char 方法"
linktitle: "CreateSafeSheetName"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CellsHelper_CreateSafeSheetName_String_Char 方法。封装了在 Go 中表示 createsafesheetname 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/cellshelper/cellshelper_createsafesheetname_string_char/
---

## CellsHelper_CreateSafeSheetName_String_Char function

检查给定的工作表名称，并在需要时创建有效名称。如果给定的工作表名称符合 Excel 工作表名称规则，则返回该名称。否则，如果长度超过限制，则会截断字符串，并将无效字符替换为给定的字符，然后返回重建后的字符串值。

```go

func CellsHelper_CreateSafeSheetName_String_Char(nameproposal string, replacechar byte)  (string,  error) 

```

## 备注


## 另请参阅

* Class [CellsHelper](../)
* Library [Aspose.Cells for Go](../../)
