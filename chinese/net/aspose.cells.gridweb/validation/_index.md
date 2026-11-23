---
title: "类 Validation"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Validation 类。"
type: docs
url: /zh/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Validation](validation/#constructor)() | 默认构造函数。 |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | 获取对象的相对单元格。（继承自 [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/)。） |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | 获取或设置客户端验证 JavaScript 函数名称。 |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | 获取或设置验证操作类型，Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual。 |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | 获取或设置运算符目标值 1。 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | 获取或设置运算符目标值 2。 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | 获取或设置单元格值是否为必填。 |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | 获取或设置正则表达式字符串。 |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | 获取值列表对象。 |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | 仅在设计时使用。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | 从 DataView 对象加载值列表。您可以指定 DataView 的值字段和文本字段。每个值和文本对将合并为一个字符串，之间用逗号分隔。 |

### 备注

注意：此类已过时。请改用 GridValidation。自 2014 年 8 月起 6 个月后此类将被移除。Aspose 对您可能遇到的任何不便表示歉意。

### 另请参见

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


