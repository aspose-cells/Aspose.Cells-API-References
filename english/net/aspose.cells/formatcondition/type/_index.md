---
title: FormatCondition.Type
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets whether the conditional format Type
type: docs
url: /net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Gets and sets whether the conditional format Type.

```csharp
public FormatConditionType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(fcs[0].Type, FormatConditionType.DataBar);
[Test]
        public void Property_Type()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47217_databar.ods");
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.DataBar);
            Assert.AreEqual(FormatConditionValueType.AutomaticMin, fcs[0].DataBar.MinCfvo.Type);
            workbook.Save(Constants.destPath + "CellsNet47217_databar.ods");
            workbook = new Workbook(Constants.destPath + "CellsNet47217_databar.ods");
            fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            Assert.AreEqual(fcs[0].Type, FormatConditionType.DataBar);
            Assert.AreEqual(FormatConditionValueType.AutomaticMin, fcs[0].DataBar.MinCfvo.Type);
        }
```

### See Also

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


