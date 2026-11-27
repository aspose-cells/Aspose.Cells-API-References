---
title: "PivotTable.PivotFilters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable egenskap. Returnerar alla filter i pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/pivotfilters/
---
## PivotTable.PivotFilters property

Returnerar alla filter i pivottabellen.

```csharp
public PivotFilterCollection PivotFilters { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyPivotFiltersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Skapa en pivottabell
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Lägg till fält i pivottabellen
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Åtkomst till PivotFilters‑samlingen (skrivskyddad egenskap)
                PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

                // Visa information om PivotFilters‑samlingen
                Console.WriteLine("Number of PivotFilters: " + pivotFilters.Count);

                // Iterera genom filtren och visa deras typer
                for (int i = 0; i < pivotFilters.Count; i++)
                {
                    PivotFilter filter = pivotFilters[i];
                    Console.WriteLine($"Filter {i + 1} Type: {filter.FilterType}");
                }

                // Lägg till ett exempelfilter för att demonstrera funktionaliteten
                if (pivotFilters.Count == 0)
                {
                    // Lägg till ett värdefilter till det första fältet (Sales)
                    PivotFilter valueFilter = pivotFilters.AddValueFilter(0, 1,
                        PivotFilterType.ValueGreaterThan, 150.0, 0.0);
                    Console.WriteLine("Added value filter: Greater than 150");
                }

                // Visa uppdaterat filterantal
                Console.WriteLine("Updated number of PivotFilters: " + pivotFilters.Count);

                // Spara arbetsboken
                workbook.Save("PivotFiltersDemo.xlsx");
                Console.WriteLine("PivotFilters demonstration completed successfully.");
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

* class [PivotFilterCollection](../../pivotfiltercollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


