---
title: "LoadFilter.LoadDataFilterOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadFilter-Eigenschaft. Die Filteroptionen, die angeben, welche Daten geladen werden sollen"
type: docs
url: /de/net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

Die Filteroptionen, die angeben, welche Daten geladen werden sollen.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertyLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = 123;
            worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

            try
            {
                // Erstellen Sie eine LoadFilter-Instanz mit Standardoptionen
                LoadFilter loadFilter = new LoadFilter();

                // Zeigen Sie den Standardwert von LoadDataFilterOptions an
                Console.WriteLine("Default LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Setzen Sie neue Filteroptionen (Kombination von Flags)
                loadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellValue | LoadDataFilterOptions.Formula;

                // Zeigen Sie den aktualisierten Wert an
                Console.WriteLine("Updated LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Erstellen Sie einen weiteren Filter mit anderen Optionen
                LoadFilter anotherFilter = new LoadFilter(LoadDataFilterOptions.Chart | LoadDataFilterOptions.Picture);

                // Zeigen Sie die Optionen aus dem Konstruktor an
                Console.WriteLine("Constructor LoadDataFilterOptions: " + anotherFilter.LoadDataFilterOptions);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


