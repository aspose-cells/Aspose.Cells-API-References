---
title: DataBar.MaxLength
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Represents the max length of data bar 
type: docs
url: /net/aspose.cells/databar/maxlength/
---
## DataBar.MaxLength property

Represents the max length of data bar .

```csharp
public int MaxLength { get; set; }
```

### Examples

```csharp
// Called: dataBar.MaxLength = 90;
public static void Property_MaxLength()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Add conditional formatting to the worksheet
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Define a cell area for the conditional formatting
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Add a data bar conditional formatting rule
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // Access the DataBar object
            DataBar dataBar = fc.DataBar;

            // Set the color of the data bar
            dataBar.Color = Color.Blue;

            // Set the minimum and maximum length of the data bar
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Set the border type of the data bar
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Set the border color of the data bar
            dataBar.BarBorder.Color = Color.Red;

            // Save the workbook
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
```

### See Also

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


