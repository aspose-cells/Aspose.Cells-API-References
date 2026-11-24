---
title: "Aufzählung SaveElementType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Saving.SaveElementType enum. Gibt an, welche Art von Elementen gespeichert werden sollen."
type: docs
url: /de/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

Stellt dar, welche Art von Elementen gespeichert werden sollen.

```csharp
public enum SaveElementType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| All | `251658239` | Alle Daten. |
| Chart | `256` | Nur Diagramme. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge einige Beispieldaten hinzu, um das Speichern zu demonstrieren
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // Erstelle ein Diagramm, um den Chart‑Speicherelementtyp zu demonstrieren
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // Demonstrieren Sie die Verwendung von SaveElementType-Enumwerten
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // Speichern Sie die Arbeitsmappe mit allen Elementen
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


