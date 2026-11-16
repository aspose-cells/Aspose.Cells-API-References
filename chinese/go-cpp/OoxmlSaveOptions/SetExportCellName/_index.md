---
title: "SetExportCellName 方法"
linktitle: "SetExportCellName"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SetExportCellName 方法。封装了在 Go 中表示 setexportcellname 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/ooxmlsaveoptions/setexportcellname/
---

## SetExportCellName function

指示是否将单元格名称导出到 Excel2007 .xlsx（.xlsm、.xltx、.xltm）文件。如果输出文件可能被 SQL Server DTS 访问，则此值必须为 true。将该值设置为 false 将大幅提升性能并在创建大文件时减小文件大小。默认值为 true。

```go

func (instance *OoxmlSaveOptions) SetExportCellName(value bool)  error

```

## 备注


## 另请参阅

* Class [OoxmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
