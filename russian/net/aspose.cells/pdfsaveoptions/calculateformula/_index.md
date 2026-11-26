---
title: "PdfSaveOptions.CalculateFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Указывает, следует ли вычислять формулы перед сохранением PDF‑файла"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

Указывает, следует ли вычислять формулы перед сохранением PDF‑файла.

```csharp
public bool CalculateFormula { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу с образцовыми данными и формулами
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить значения и формулы
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Создайте параметры сохранения PDF с вычислением формул
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            // Сохранить в поток памяти
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Сбросьте позицию потока и проверьте содержимое
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine("PDF contains formula results: " + content.Contains("30"));
                }
            }
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


