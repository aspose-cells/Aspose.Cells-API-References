---
title: "GetStringValue 方法"
linktitle: "GetStringValue"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetStringValue 方法。封装了在 Go 中表示 getstringvalue 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/cell/getstringvalue/
---

## GetStringValue function

获取单元格中的字符串值。如果此单元格的类型是字符串，则返回字符串本身。对于其他单元格类型，将返回格式化的字符串值（使用此单元格的指定样式进行格式化）。格式化后的单元格值与在 Excel 中将单元格复制为文本时（例如复制到文本编辑器或导出为 CSV）获得的值相同。

```go

func (instance *Cell) GetStringValue()  (string,  error) 

```

## 备注


## 另请参阅

* Class [Cell](../)
* Library [Aspose.Cells for Go](../../)
