---
title: Equals
second_title: Aspose.Cells for .NET API 参考
description: 确定此实例是否与另一个指定的值相同ShapeTextAlignmentaspose.cells.drawing.texts/shapetextalignment对象.
type: docs
weight: 140
url: /zh/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

确定此实例是否与另一个指定的值相同[`ShapeTextAlignment`](../../shapetextalignment)对象.

```csharp
public override bool Equals(object obj)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| obj | Object | 这[`ShapeTextAlignment`](../../shapetextalignment)要与此实例进行比较的对象。 |

### 返回值

如果 obj 参数的值与此实例的值相同，则为 true；否则为假。如果 obj 为 null，则此方法返回 false。

### 例子

```csharp

[C#]
//你要确保这行代码中的索引值存在
Aspose.Cells.Drawing.Texts.ShapeTextAlignment obj = workbook.Worksheets[0].Shapes[0].TextBody.TextAlignment;
if (shapeTextAlignment.Equals(obj))
{
    //做你想做的
}
```

### 也可以看看

* class [ShapeTextAlignment](../../shapetextalignment)
* 命名空间 [Aspose.Cells.Drawing.Texts](../../shapetextalignment)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
