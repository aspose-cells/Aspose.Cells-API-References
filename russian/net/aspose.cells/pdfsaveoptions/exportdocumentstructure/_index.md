---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Указывает, следует ли экспортировать структуру документа"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Указывает, следует ли экспортировать структуру документа.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Установите ExportDocumentStructure в true, чтобы сохранить структуру документа
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // Вычислить формулы перед сохранением
            workbook.CalculateFormula();

            // Сохраните книгу в PDF с указанными параметрами
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


