---
title: AboveAverage.StdDev
second_title: Aspose.Cells for .NET API Reference
description: AboveAverage property. Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 include 0 and 3. Setting this value to 0 means stdDev is not set. The default value is 0
type: docs
url: /net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0.

```csharp
public int StdDev { get; set; }
```

### Examples

```csharp
// Called: fc.AboveAverage.StdDev = 2;
public static void Property_StdDev()
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
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Adds a condition for ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Save the Excel file
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
```

### See Also

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


