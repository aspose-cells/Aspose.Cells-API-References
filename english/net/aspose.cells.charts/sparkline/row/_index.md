---
title: Sparkline.Row
second_title: Aspose.Cells for .NET API Reference
description: Sparkline property. Gets the row index of the sparkline
type: docs
url: /net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Gets the row index of the sparkline.

```csharp
public int Row { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);
public static void Sparkline_Property_Row()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Add a sparkline to the group
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline line = group.Sparklines[idx];

            // Output sparkline details
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Save the sparkline as an image
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Save the workbook
            workbook.Save("SparklineExample.xlsx");
        }
```

### See Also

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


