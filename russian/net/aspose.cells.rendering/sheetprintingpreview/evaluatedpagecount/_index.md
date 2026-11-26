---
title: "SheetPrintingPreview.EvaluatedPageCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SheetPrintingPreview. Оценивает общее количество страниц этого листа"
type: docs
url: /ru/net/aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/
---
## SheetPrintingPreview.EvaluatedPageCount property

Оцените общее количество страниц этого листа

```csharp
public int EvaluatedPageCount { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            Console.WriteLine("Evaluated Page Count: " + preview.EvaluatedPageCount);
        }
    }
}
```

### См. также

* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


