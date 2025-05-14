---
title: FormatCondition.IconSet
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings IconSet instance. The default instances IconSetType is TrafficLights31. Valid only for type  IconSet
type: docs
url: /net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Examples

```csharp
// Called: ConditionalFormattingIconCollection iconCollection = condition.IconSet.CfIcons;
public void FormatCondition_Property_IconSet()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/TestConditionalIcon1.xlsx");
    Worksheet sheet1 = workbook.Worksheets[0];
    ConditionalFormattingResult r = sheet1.Cells["C2"].GetConditionalFormattingResult();
    Assert.AreEqual(r.ConditionalFormattingIcon.Index, 2);
    r = sheet1.Cells["D2"].GetConditionalFormattingResult();
    Assert.AreEqual(r.ConditionalFormattingIcon.Index, 1);
    r = sheet1.Cells["E2"].GetConditionalFormattingResult();
    Assert.AreEqual(r.ConditionalFormattingIcon.Index, 0);
    FormatConditionCollection conditionCollection = sheet1.ConditionalFormattings[0];
    FormatCondition condition = conditionCollection[0];
        
    ConditionalFormattingIconCollection iconCollection = condition.IconSet.CfIcons;
    Assert.AreEqual(0, iconCollection[0].Index);
    Assert.AreEqual(1, iconCollection[1].Index);
    Assert.AreEqual(2, iconCollection[2].Index);

}
```

### See Also

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


