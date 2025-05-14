---
title: FormatCondition.ColorScale
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings ColorScale instance. The default instance is a greenyellowred 3ColorScale . Valid only for type  ColorScale
type: docs
url: /net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(FormatConditionValueType.Min, fcs[0].ColorScale.MinCfvo.Type);
public void FormatCondition_Property_ColorScale()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
    Assert.AreEqual(fcs[0].Type, FormatConditionType.ColorScale);
    Assert.AreEqual(FormatConditionValueType.Min, fcs[0].ColorScale.MinCfvo.Type);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    fcs = workbook.Worksheets[0].ConditionalFormattings[0];
    Assert.AreEqual(fcs[0].Type, FormatConditionType.ColorScale);
    Assert.AreEqual(FormatConditionValueType.Min, fcs[0].ColorScale.MinCfvo.Type);
}
```

### See Also

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


