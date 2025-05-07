---
title: FormatCondition.Style
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets or setts style of conditional formatted cell ranges
type: docs
url: /net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

Gets or setts style of conditional formatted cell ranges.

```csharp
public Style Style { get; set; }
```

### Examples

```csharp
// Called: Style style = formatCondition.Style;
[Test]
        public void Property_Style()
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
            book.Save(Constants.destPath + "CellsJava40335.xlsx");
            book = new Workbook(Constants.destPath + "CellsJava40335.xlsx");
            Assert.AreEqual("вс", book.Worksheets[0].ConditionalFormattings[0][0].Text);
            book.Save(Constants.destPath + "dest.xls");
            book = new Workbook(Constants.destPath + "dest.xls");
            Assert.AreEqual("вс", book.Worksheets[0].ConditionalFormattings[0][0].Text);
        }
```

### See Also

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


