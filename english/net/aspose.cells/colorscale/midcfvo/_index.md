---
title: ColorScale.MidCfvo
second_title: Aspose.Cells for .NET API Reference
description: ColorScale property. Get or set this ColorScales mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it
type: docs
url: /net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(50, (int)sheet.ConditionalFormattings[0][0].ColorScale.MidCfvo.Value);
public void ColorScale_Property_MidCfvo()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet = workbook.Worksheets[4];
           
    Assert.AreEqual(50, (int)sheet.ConditionalFormattings[0][0].ColorScale.MidCfvo.Value);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


