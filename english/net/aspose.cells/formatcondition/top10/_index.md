---
title: FormatCondition.Top10
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings Top10 instance. The default instances rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10
type: docs
url: /net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10.

```csharp
public Top10 Top10 { get; }
```

### Examples

```csharp
// Called: Top10 top10 = fc.Top10;
public static void Property_Top10()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Sets the conditional format range
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Adds condition
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Setting properties
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Saving the Excel file
            workbook.Save("Top10Example.xlsx");
        }
```

### See Also

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


