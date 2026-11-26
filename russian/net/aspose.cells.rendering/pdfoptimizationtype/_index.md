---
title: "Перечисление PdfOptimizationType."
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.PdfOptimizationType. Указывает тип оптимизации."
type: docs
url: /ru/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

Указывает тип оптимизации.

```csharp
public enum PdfOptimizationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Standard | `0` | Высокое качество печати. |
| MinimumSize | `1` | Размер файла важнее качества печати. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfOptimizationTypeDemo
    {
        public static void PdfOptimizationTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Создайте PdfSaveOptions и задайте тип оптимизации.
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Сохраните книгу в формате PDF с указанным типом оптимизации.
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


