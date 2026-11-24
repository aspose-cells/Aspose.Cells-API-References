---
title: "Workbook.MergeNamedStyles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Führt benannte Stile aus der anderen Excel-Datei zusammen"
type: docs
url: /de/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Führt benannte Stile aus der anderen Excel‑Datei zusammen.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Arbeitsmappe | Die andere Datei |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Erstelle die Zielarbeitsmappe (diejenige, die benannte Stile erhalten wird)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Füge der Zielarbeitsmappe einige Daten zum Kontext hinzu
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Erstelle die Quellarbeitsmappe (diejenige, die zu mergende benannte Stile enthält)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Füge der Quellarbeitsmappe einige Daten zum Kontext hinzu
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // Führe benannte Stile von sourceWorkbook in targetWorkbook zusammen
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Speichere die resultierende Arbeitsmappe
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


