---
title: PivotDateTimeRangeGroupSettings.GroupByTypes
second_title: Aspose.Cells for .NET API Reference
description: PivotDateTimeRangeGroupSettings property. Gets the types of grouping by date time
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/
---
## PivotDateTimeRangeGroupSettings.GroupByTypes property

Gets the types of grouping by date time.

```csharp
public PivotGroupByType[] GroupByTypes { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDateTimeRangeGroupSettingsPropertyGroupByTypesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with dates
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Create pivot table
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Add fields to pivot table
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Group by date with multiple grouping types
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                PivotGroupByType[] groupTypes = new PivotGroupByType[]
                {
                    PivotGroupByType.Months,
                    PivotGroupByType.Quarters
                };
                dateField.GroupBy(startDate, endDate, groupTypes, 1, false);

                // Access the group settings and demonstrate GroupByTypes property
                PivotDateTimeRangeGroupSettings groupSettings =
                    (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Display the GroupByTypes property value
                Console.WriteLine("GroupByTypes values:");
                foreach (PivotGroupByType type in groupSettings.GroupByTypes)
                {
                    Console.WriteLine(type);
                }

                // Save the result
                workbook.Save("GroupByTypesDemo.xlsx");
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

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


