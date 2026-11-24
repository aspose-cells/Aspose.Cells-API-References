---
title: "LoadOptions.LoadFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt das Ladeformat zurück"
type: docs
url: /de/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

Liest das Ladeformat.

```csharp
public LoadFormat LoadFormat { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Erstelle Beispiel-CSV-Datei
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // Erstelle LoadOptions für das CSV-Format und zeige die Eigenschaft an
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // Lade CSV mit den richtigen Optionen
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // Erstelle LoadOptions für das XLSX-Format und zeige die Eigenschaft an
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // Erstelle/speichere Beispiel-XLSX-Datei
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // Lade XLSX mit den richtigen Optionen
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // Bereinige temporäre Dateien
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


