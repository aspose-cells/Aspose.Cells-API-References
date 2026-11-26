---
title: "Перечисление SlideViewType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Slides.SlideViewType. Представляет тип при экспорте в слайды"
type: docs
url: /ru/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Представляет тип при экспорте в слайды.

```csharp
public enum SlideViewType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| View | `0` | Экспорт в виде представления в MS Excel. |
| Print | `1` | Экспорт в виде печати. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassSlideViewTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // Настройте параметры сохранения PPTX с помощью SlideViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // Сохранить как PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


