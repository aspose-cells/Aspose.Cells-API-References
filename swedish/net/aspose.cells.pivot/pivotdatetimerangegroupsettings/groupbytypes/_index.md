---
title: "PivotDateTimeRangeGroupSettings.GroupByTypes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotDateTimeRangeGroupSettings‑egenskap. Hämtar typerna av gruppering efter datum och tid"
type: docs
url: /sv/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/
---
## PivotDateTimeRangeGroupSettings.GroupByTypes property

Hämtar typerna av gruppering efter datum och tid.

```csharp
public PivotGroupByType[] GroupByTypes { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med datum
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
                // Skapa pivottabell
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Lägg till fält i pivottabell
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Gruppera efter datum med flera grupperingstyper
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                PivotGroupByType[] groupTypes = new PivotGroupByType[]
                {
                    PivotGroupByType.Months,
                    PivotGroupByType.Quarters
                };
                dateField.GroupBy(startDate, endDate, groupTypes, 1, false);

                // Åtkomst till gruppinställningarna och demonstrera GroupByTypes‑egenskapen
                PivotDateTimeRangeGroupSettings groupSettings =
                    (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Visa värdet för GroupByTypes‑egenskapen
                Console.WriteLine("GroupByTypes values:");
                foreach (PivotGroupByType type in groupSettings.GroupByTypes)
                {
                    Console.WriteLine(type);
                }

                // Spara resultatet
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

### Se även

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


