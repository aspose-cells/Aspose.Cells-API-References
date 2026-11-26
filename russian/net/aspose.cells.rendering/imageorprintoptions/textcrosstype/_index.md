---
title: "ImageOrPrintOptions.TextCrossType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/textcrosstype/
---
## ImageOrPrintOptions.TextCrossType property

Получает или задает тип отображения текста, когда ширина текста превышает ширину ячейки.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите длинный текст, который превысит ширину ячейки
            worksheet.Cells["A1"].PutValue("This is a long text that exceeds cell width");
            worksheet.Cells["A1"].GetStyle().ShrinkToFit = false;

            // Создать параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Продемонстрировать различные настройки TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveAsImage(workbook, options, "TextCrossType_Default.png");

            options.TextCrossType = TextCrossType.CrossKeep;
            SaveAsImage(workbook, options, "TextCrossType_CrossKeep.png");

            options.TextCrossType = TextCrossType.CrossOverride;
            SaveAsImage(workbook, options, "TextCrossType_CrossOverride.png");

            options.TextCrossType = TextCrossType.StrictInCell;
            SaveAsImage(workbook, options, "TextCrossType_StrictInCell.png");
        }

        private static void SaveAsImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### См. также

* enum [TextCrossType](../../../aspose.cells/textcrosstype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


