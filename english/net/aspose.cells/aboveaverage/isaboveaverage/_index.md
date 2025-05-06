---
title: AboveAverage.IsAboveAverage
second_title: Aspose.Cells for .NET API Reference
description: AboveAverage property. Get or set the flag indicating whether the rule is an above average rule. true indicates above average. Default value is true
type: docs
url: /net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true.

```csharp
public bool IsAboveAverage { get; set; }
```

### Examples

```csharp
// Called: fc.AboveAverage.IsAboveAverage = true;
public static void Property_IsAboveAverage()
        {
            // Create a new Workbook.
            Workbook workbook = new Workbook();

            // Get the first worksheet.
            Worksheet worksheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Sets the conditional format range.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Adds a condition for AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Setting properties for AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Adds a condition for CellValue
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, &quot;50&quot;, &quot;100&quot;);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Adds a condition for ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = &quot;Sample&quot;;
            fc3.Style.BackgroundColor = Color.Green;

            // Save the Excel file
            workbook.Save(&quot;FormatConditionTypeExample.xlsx&quot;);
            workbook.Save(&quot;FormatConditionTypeExample.pdf&quot;);
        }
```

### See Also

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


