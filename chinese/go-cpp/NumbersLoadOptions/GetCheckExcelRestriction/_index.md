---
title: "GetCheckExcelRestriction 方法"
linktitle: "GetCheckExcelRestriction"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetCheckExcelRestriction 方法。封装了在 Go 中表示 getcheckexcelrestriction 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/numbersloadoptions/getcheckexcelrestriction/
---

## GetCheckExcelRestriction function

是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。

```go

func (instance *NumbersLoadOptions) GetCheckExcelRestriction()  (bool,  error) 

```

## 备注


## 另请参阅

* Class [NumbersLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
