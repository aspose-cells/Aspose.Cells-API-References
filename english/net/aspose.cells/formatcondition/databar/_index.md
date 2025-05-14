---
title: FormatCondition.DataBar
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings DataBar instance. The default instances color is blue. Valid only for type is DataBar
type: docs
url: /net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.

```csharp
public DataBar DataBar { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(FormatConditionValueType.AutomaticMin, fcs[0].DataBar.MinCfvo.Type);
public void FormatCondition_Property_DataBar()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
    Assert.AreEqual(fcs[0].Type, FormatConditionType.DataBar);
    Assert.AreEqual(FormatConditionValueType.AutomaticMin, fcs[0].DataBar.MinCfvo.Type);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    fcs = workbook.Worksheets[0].ConditionalFormattings[0];
    Assert.AreEqual(fcs[0].Type, FormatConditionType.DataBar);
    Assert.AreEqual(FormatConditionValueType.AutomaticMin, fcs[0].DataBar.MinCfvo.Type);
}
```

### See Also

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


