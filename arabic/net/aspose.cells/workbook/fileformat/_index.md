---
title: "Workbook.FileFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل وتضبط تنسيق الملف"
type: docs
url: /ar/net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

يحصل على ويضبط تنسيق الملف.

```csharp
public FileFormatType FileFormat { get; set; }
```

### أمثلة

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
            // إنشاء ملف CSV تجريبي
            string csvFile = "sample.csv";
            File.WriteAllText(csvFile, "Name,Age\nJohn,30\nJane,25");

            // إنشاء ملف XLSX تجريبي
            string xlsxFile = "sample.xlsx";
            using (Workbook wb = new Workbook())
            {
                wb.Worksheets[0].Cells["A1"].PutValue("Test");
                wb.Save(xlsxFile);
            }

            // توضيح خاصية FileFormat
            ProcessWorkbook(csvFile);
            ProcessWorkbook(xlsxFile);

            // تنظيف
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
                    // معالجة إضافية خاصة بـ CSV
                }
                else if (wb.FileFormat == FileFormatType.Xlsx)
                {
                    Console.WriteLine("This is an XLSX file");
                    // معالجة إضافية خاصة بـ XLSX
                }
            }
        }
    }
}
```

### انظر أيضًا

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


