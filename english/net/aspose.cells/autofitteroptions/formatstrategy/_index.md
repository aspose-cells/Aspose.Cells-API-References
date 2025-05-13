---
title: AutoFitterOptions.FormatStrategy
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and sets the formatted strategy
type: docs
url: /net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Gets and sets the formatted strategy.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Remarks

The default value is CellStyle for performance.

### Examples

```csharp
// Called: FormatStrategy = CellValueFormatStrategy.DisplayString,
public static void AutoFitterOptions_Property_FormatStrategy()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // Create a range A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Merge the cells
            range.Merge();

            // Create an instance of AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Apply auto fit rows with the specified options
            worksheet.AutoFitRows(options);

            // Save the workbook
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
```

### See Also

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


