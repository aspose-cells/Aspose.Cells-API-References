---
title: "Перечисление TextCrossType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TextCrossType. Перечисляет тип отображения текста, когда ширина текста превышает ширину ячейки"
type: docs
url: /ru/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Перечисляет типы отображения текста, когда ширина текста превышает ширину ячейки.

```csharp
public enum TextCrossType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `1` | Отображать текст так же, как в Microsoft Excel. |
| CrossKeep | `2` | Отображать весь текст, пересекающий другие ячейки, и сохранять текст пересечённых ячеек. |
| CrossOverride | `3` | Отображать весь текст, пересекающий другие ячейки, и переопределять текст пересекаемых ячеек. |
| StrictInCell | `4` | Отображать только текст в пределах ширины ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassTextCrossTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить пример текста в ячейку, который может выходить за пределы.
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // Создать параметры изображения или печати
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Продемонстрировать различные настройки TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveToImage(workbook, options, "TextCrossType_Default.png");
            
            options.TextCrossType = TextCrossType.CrossKeep;
            SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
            
            options.TextCrossType = TextCrossType.CrossOverride;
            SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
            
            options.TextCrossType = TextCrossType.StrictInCell;
            SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
        }
        
        private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


