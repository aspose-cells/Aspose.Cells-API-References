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
// Called: Assert.AreEqual("вс", formatCondition.Text);
public void FormatCondition_Property_Text()
{
    Workbook book = new Workbook();
    Worksheet sheet = book.Worksheets[0];
    ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
    int collectionIndex = conditionalFormattings.Add();
    FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];
    int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
    FormatCondition formatCondition = formatConditions[conditionIndex];
    formatCondition.Text = ("вс");  // Note: this is Russian and not English ("вс" != "BC")
    Style style = formatCondition.Style;
    style.BackgroundColor = Color.Red;// (Color.getRed());
    formatCondition.Style = (style);
    formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));
    Assert.AreEqual("вс", formatCondition.Text);
    book.Save(Constants.destPath + "example.xlsx");
    book = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual("вс", book.Worksheets[0].ConditionalFormattings[0][0].Text);
    book.Save(Constants.destPath + "dest.xls");
    book = new Workbook(Constants.destPath + "dest.xls");
    Assert.AreEqual("вс", book.Worksheets[0].ConditionalFormattings[0][0].Text);
}
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


