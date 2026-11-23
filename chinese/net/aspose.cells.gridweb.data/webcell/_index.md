---
title: "类 WebCell"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.WebCell 类。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webcell/
---
## WebCell class

```csharp
[Obsolete("This class is obsolete; use  GridCell instead")]
public class WebCell
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Column](../../aspose.cells.gridweb.data/webcell/column/) { get; } | 获取单元格的列号。 |
| [Formula](../../aspose.cells.gridweb.data/webcell/formula/) { get; set; } | 获取或设置单元格的公式字符串。如果单元格不包含公式，则返回 null。 |
| [IsReadonly](../../aspose.cells.gridweb.data/webcell/isreadonly/) { get; set; } | 获取或设置单元格是否只读。这是 GridWeb 的扩展属性，实际 Excel 文件中不会保留。 |
| [Name](../../aspose.cells.gridweb.data/webcell/name/) { get; } |  |
| [Row](../../aspose.cells.gridweb.data/webcell/row/) { get; } | 获取单元格的行号。 |
| [StringValue](../../aspose.cells.gridweb.data/webcell/stringvalue/) { get; set; } |  |
| [UnformattedStringValue](../../aspose.cells.gridweb.data/webcell/unformattedstringvalue/) { get; } | 获取未格式化的字符串值。 |
| [Validation](../../aspose.cells.gridweb.data/webcell/validation/) { get; set; } |  |
| [Value](../../aspose.cells.gridweb.data/webcell/value/) { get; set; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetStyle](../../aspose.cells.gridweb.data/webcell/getstyle/)() |  |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue)(bool) | 将布尔值放入单元格。 |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue_3)(DateTime) | 将 DateTime 值放入单元格。 |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue_1)(double) | 将 double 值放入单元格。 |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue_2)(int) | 将 int 值放入单元格。 |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue_4)(object) | 将对象值放入单元格。与 setValue(Object param_object) 相同。 |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue_5)(string) | 将 String 值放入单元格。 |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue_6)(string, bool) | 将字符串值放入单元格，并在适当时将该值转换为其他数据类型。 |
| [PutValue](../../aspose.cells.gridweb.data/webcell/putvalue/#putvalue_7)(string, bool, bool) | 将值放入单元格，如有必要，该值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/webcell/putvalueandsetformatbyvalue/)(string) | 使用字符串值设置单元格的值，并根据该值设置单元格格式。 |
| [SetStyle](../../aspose.cells.gridweb.data/webcell/setstyle/)(TableItemStyle) |  |

### 备注

注意：此类现已过时。请改用 GridCell。自 2014 年 8 月起 6 个月后此类将被移除。Aspose 对您可能遇到的任何不便表示歉意。

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


