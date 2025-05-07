---
title: FormatCondition.Text
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. The text value in a text contains conditional formatting rule. Valid only for type  containsText notContainsText beginsWith and endsWith. The default value is null
type: docs
url: /net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

```csharp
public string Text { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[0].ConditionalFormattings[0][0].Text,"\"\"");
[Test]
        public void Property_Text()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].ConditionalFormattings.Add();
            FormatConditionCollection fcs = wb.Worksheets[0].ConditionalFormattings[0];
            fcs.Add(CellArea.CreateCellArea("A1", "A10"), FormatConditionType.ContainsText, OperatorType.None, null, null);
            fcs[0].Text = "\"\"";
            wb.Save(Constants.destPath + "Cellsnet42920.xlsx");
            wb = new Workbook(Constants.destPath + "Cellsnet42920.xlsx");
           Assert.AreEqual(wb.Worksheets[0].ConditionalFormattings[0][0].Text,"\"\"");
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


