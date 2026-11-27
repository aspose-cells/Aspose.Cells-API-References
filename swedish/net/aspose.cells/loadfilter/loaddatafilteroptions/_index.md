---
title: "LoadFilter.LoadDataFilterOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadFilter‑egenskap. Filteralternativen som anger vilken data som ska laddas"
type: docs
url: /sv/net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

Filteralternativen för att ange vilken data som ska läsas in.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertyLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = 123;
            worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

            try
            {
                // Skapa en LoadFilter‑instans med standardalternativ
                LoadFilter loadFilter = new LoadFilter();

                // Visa standardvärdet för LoadDataFilterOptions
                Console.WriteLine("Default LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Ställ in nya filteralternativ (kombination av flaggor)
                loadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellValue | LoadDataFilterOptions.Formula;

                // Visa det uppdaterade värdet
                Console.WriteLine("Updated LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Skapa ett annat filter med olika alternativ
                LoadFilter anotherFilter = new LoadFilter(LoadDataFilterOptions.Chart | LoadDataFilterOptions.Picture);

                // Visa alternativen från konstruktorn
                Console.WriteLine("Constructor LoadDataFilterOptions: " + anotherFilter.LoadDataFilterOptions);

                // Spara arbetsboken
                workbook.Save("LoadDataFilterOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


