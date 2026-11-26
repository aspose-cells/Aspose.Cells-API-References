---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор SheetPrintingPreview. Конструкция SheetPrintingPreview"
type: docs
url: /ru/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

Конструкция SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| лист | Worksheet | Укажите, какая таблица будет печататься. |
| опции | ImageOrPrintOptions | ImageOrPrintOptions содержит некоторые свойства вывода |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Создать параметры изображения/печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Создайте предварительный просмотр печати листа
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // Выведите рассчитанное количество страниц
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### См. также

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


