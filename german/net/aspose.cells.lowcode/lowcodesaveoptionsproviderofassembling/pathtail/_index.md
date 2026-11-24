---
title: "LowCodeSaveOptionsProviderOfAssembling.PathTail"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling property. Nachgestellter Teil nach den Sequenznummern des Dateipfads. Er sollte die Dateierweiterung enthalten"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/
---
## LowCodeSaveOptionsProviderOfAssembling.PathTail property

Nachtrag (nach den Sequenznummern) des Dateipfads. Er sollte die Dateinamenerweiterung enthalten.

```csharp
public string PathTail { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathTailDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit Beispieldaten erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Record {i + 1}";
            }

            // Speicheroptionen‑Anbieter initialisieren
            var optionsProvider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SalesReports/Q3",
                PathTail = ".xlsx",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            Console.WriteLine($"Original file extension: {optionsProvider.PathTail}");

            // Erste Speicherung mit Standarderweiterung
            workbook.Save("output_original", optionsProvider.SaveOptionsTemplate.SaveFormat);

            // Pfadnachlauf für CSV‑Ausgabe ändern
            optionsProvider.PathTail = "_split.csv";
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Csv;
            Console.WriteLine($"Modified file extension: {optionsProvider.PathTail}");

            // Zweite Speicherung mit neuer Erweiterung
            workbook.Save("output_modified", optionsProvider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check output directories for generated file formats");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


