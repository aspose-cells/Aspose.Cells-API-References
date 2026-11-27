---
title: "PivotField.GetPivotFilters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Hämtar pivottfiltren för pivottfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/getpivotfilters/
---
## PivotField.GetPivotFilters method

Hämtar pivottfiltren för pivottfältet

```csharp
[Obsolete("Use PivotField.GetFilters() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetPivotFilters()
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.GetFilters()‑metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotFieldMethodGetPivotFiltersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Skapa en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till pivottfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Anropa GetPivotFilters‑metoden (föråldrad)
                ArrayList pivotFilters = pivotField.GetPivotFilters();
                
                Console.WriteLine($"Number of pivot filters: {pivotFilters.Count}");
                
                // Alternativt, använd den icke‑föråldrade GetFilters()-metoden
                PivotFilter[] filters = pivotField.GetFilters();
                Console.WriteLine($"Number of filters (non-obsolete method): {filters.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPivotFilters method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodGetPivotFiltersDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


