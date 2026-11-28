---
title: "Workbook.FileFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Dosya formatını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Dosya biçimini alır ve ayarlar.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Örnekler

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
            // Örnek bir CSV dosyası oluşturun
            string csvFile = "sample.csv";
            File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");

            // Örnek bir XLSX dosyası oluşturun
            string xlsxFile = "sample.xlsx";
            using (Workbook wb = new Workbook())
            {
                wb.Worksheets[0].Cells["A1"].PutValue("Test");
                wb.Save(xlsxFile);
            }

            // FileFormat özelliğini gösterin
            ProcessWorkbook(csvFile);
            ProcessWorkbook(xlsxFile);

            // Temizleme
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
                    // Ek CSV-özel işleme
                }
                else if (wb.FileFormat == FileFormatType.Xlsx)
                {
                    Console.WriteLine("This is an XLSX file");
                    // Ek XLSX-özel işleme
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


