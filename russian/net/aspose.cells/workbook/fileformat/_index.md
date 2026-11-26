---
title: "Workbook.FileFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает и задает формат файла"
type: docs
url: /ru/net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Получает и задает формат файла.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Примеры

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
            // Создайте пример CSV‑файла
            string csvFile = "sample.csv";
            File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");

            // Создайте пример XLSX‑файла
            string xlsxFile = "sample.xlsx";
            using (Workbook wb = new Workbook())
            {
                wb.Worksheets[0].Cells["A1"].PutValue("Test");
                wb.Save(xlsxFile);
            }

            // Продемонстрировать свойство FileFormat
            ProcessWorkbook(csvFile);
            ProcessWorkbook(xlsxFile);

            // Очистка
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
                    // Дополнительная обработка, специфичная для CSV
                }
                else if (wb.FileFormat == FileFormatType.Xlsx)
                {
                    Console.WriteLine("This is an XLSX file");
                    // Дополнительная обработка, специфичная для XLSX
                }
            }
        }
    }
}
```

### См. также

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


