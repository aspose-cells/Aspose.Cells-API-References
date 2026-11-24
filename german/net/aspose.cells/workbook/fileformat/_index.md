---
title: "Workbook.FileFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt das Dateiformat zurück und legt es fest"
type: docs
url: /de/net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Liest und setzt das Dateiformat.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileFormatDemo
    {
        public static void Run()
        {
            // Beispiel-CSV-Datei erstellen
            string csvFile = "sample.csv";
            File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");

            // Beispiel-XLSX-Datei erstellen
            string xlsxFile = "sample.xlsx";
            using (Workbook wb = new Workbook())
            {
                wb.Worksheets[0].Cells["A1"].PutValue("Test");
                wb.Save(xlsxFile);
            }

            // FileFormat-Eigenschaft demonstrieren
            ProcessWorkbook(csvFile);
            ProcessWorkbook(xlsxFile);

            // Aufräumen
            File.Delete(csvFile);
            File.Delete(xlsxFile);
        }

        private static void ProcessWorkbook(string filePath)
        {
            using (Workbook wb = new Workbook(filePath))
            {
                Console.WriteLine($"Processing file: {filePath}");
                Console.WriteLine($"File format: {wb.FileFormat}");

                if (wb.FileFormat == FileFormatType.Csv)
                {
                    Console.WriteLine("This is a CSV file");
                    // Zusätzliche CSV-spezifische Verarbeitung
                }
                else if (wb.FileFormat == FileFormatType.Xlsx)
                {
                    Console.WriteLine("This is an XLSX file");
                    // Zusätzliche XLSX-spezifische Verarbeitung
                }
            }
        }
    }
}
```

### Siehe auch

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


