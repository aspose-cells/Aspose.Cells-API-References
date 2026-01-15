---
title: DataSorterKey.IconId
second_title: Aspose.Cells for .NET API Reference
description: DataSorterKey property. Represents the id of the icon set type
type: docs
url: /net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Represents the id of the icon set type.

```csharp
public int IconId { get; }
```

### Remarks

Only takes effect when [`Type`](../type/) is Icon.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with values that could use icon sets
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Add icon set conditional formatting
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Create data sorter and add key
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Sort the data
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Display the IconId property from the sorter keys
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Save the workbook
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


