---
title: "Workbook.FileFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar och anger filformatet"
type: docs
url: /sv/net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Hämtar och anger filformatet.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Exempel

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
            // Skapa en exempel-CSV-fil
            string csvFile = "sample.csv";
            File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");

            // Skapa en exempel-XLSX-fil
            string xlsxFile = "sample.xlsx";
            using (Workbook wb = new Workbook())
            {
                wb.Worksheets[0].Cells["A1"].PutValue("Test");
                wb.Save(xlsxFile);
            }

            // Demonstrera egenskapen FileFormat
            ProcessWorkbook(csvFile);
            ProcessWorkbook(xlsxFile);

            // Städa upp
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
                    // Ytterligare CSV-specifik bearbetning
                }
                else if (wb.FileFormat == FileFormatType.Xlsx)
                {
                    Console.WriteLine("This is an XLSX file");
                    // Ytterligare XLSX-specifik bearbetning
                }
            }
        }
    }
}
```

### Se även

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


