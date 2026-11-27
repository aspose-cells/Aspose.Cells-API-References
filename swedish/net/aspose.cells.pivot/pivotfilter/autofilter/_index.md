---
title: "PivotFilter.AutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-egenskap. Hämtar autofiltret för pivottfiltret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/autofilter/
---
## PivotFilter.AutoFilter property

Hämtar autofiltret för pivottfiltret.

```csharp
[Obsolete("Use FilterLabel, FilterValue,FilterDate or FilterTop10 method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter AutoFilter { get; }
```

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället FilterLabel, FilterValue, FilterDate eller FilterTop10-metoden. Den här metoden kommer att tas bort 12 månader senare från och med november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Lägg till ett filter i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.PageFields[0];

            // Skapa och lägg till filter
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];

            try
            {
                // Visa AutoFilter-egenskapens värde (skrivskyddat)
                Console.WriteLine("AutoFilter Range: " + filter.AutoFilter.Range);
                Console.WriteLine("AutoFilter ShowFilterButton: " + filter.AutoFilter.ShowFilterButton);

                // Demonstrera åtkomst till AutoFilter-egenskaper
                Console.WriteLine("AutoFilter has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("PivotFilterAutoFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


