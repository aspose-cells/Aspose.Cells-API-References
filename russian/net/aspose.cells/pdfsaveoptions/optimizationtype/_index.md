---
title: "PdfSaveOptions.OptimizationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Получает и задает тип оптимизации PDF"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

Получает и задаёт тип оптимизации PDF.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### Примечания

Значение по умолчанию — Standard

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyOptimizationTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Продемонстрировать свойство OptimizationType
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Сохраните рабочую книгу с настройками оптимизации
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


