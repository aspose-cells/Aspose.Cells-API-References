---
title: "PivotFilter.GetLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilter-Methode. Gibt die Beschriftungen des Caption‑Filters zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfilter/getlabels/
---
## PivotFilter.GetLabels method

Ermittelt die Beschriftungen des Caption-Filters.

```csharp
public string[] GetLabels()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterMethodGetLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstellen einer gültigen Pivot‑Tabellenstruktur
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                
                // Erstelle eine Pivot-Tabelle mit den richtigen Parametern
                int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Erstellen eines Pivot‑Filters mit gültigen Parametern
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Konfigurieren der Filtereigenschaften
                pivotFilter.Name = "SampleFilter";
                pivotFilter.EvaluationOrder = 1;

                // Ausführen der GetLabels‑Methode
                string[] labels = pivotFilter.GetLabels();

                Console.WriteLine($"Retrieved {labels?.Length ?? 0} labels:");
                if (labels != null)
                {
                    foreach (string label in labels)
                    {
                        Console.WriteLine($"- {label}");
                    }
                }

                workbook.Save("GetLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLabels: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


