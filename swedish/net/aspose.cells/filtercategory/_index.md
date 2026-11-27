---
title: "Enum FilterCategory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FilterCategory enum. Representerar filterkategorin"
type: docs
url: /sv/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

Representerar filterkategorin.

```csharp
public enum FilterCategory
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen filtrering. |
| Label | `1` | Rubrikfilter. |
| NumberValue | `2` | Talvärdesfilter. |
| Date | `3` | Datumvärdesfilter. |
| Top10 | `4` | Top10-värdefilter. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            CreateSampleData(worksheet);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Konfigurera radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // Konfigurera datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Lägg till etikettfilter till pivottfilter
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // Demonstrera användning av FilterCategory
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // Visa alla filterkategorier i pivottabellen
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara resultatet
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Ange rubriker för exempeldata
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // Lägg till rader med exempeldata
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


