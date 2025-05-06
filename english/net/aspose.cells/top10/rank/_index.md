---
title: Top10.Rank
second_title: Aspose.Cells for .NET API Reference
description: Top10 property. Get or set the value of n in a top/bottom n conditional formatting rule. If IsPercent is true the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10
type: docs
url: /net/aspose.cells/top10/rank/
---
## Top10.Rank property

Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10.

```csharp
public int Rank { get; set; }
```

### Examples

```csharp
// Called: top10.Rank = 5;
public static void Property_Rank()
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
            workbook.Save(&quot;Top10Example.xlsx&quot;);
        }
```

### See Also

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


