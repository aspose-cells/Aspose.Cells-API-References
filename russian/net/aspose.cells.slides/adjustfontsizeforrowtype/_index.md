---
title: "Перечисление AdjustFontSizeForRowType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Slides.AdjustFontSizeForRowType. Представляет, какие типы строк должны быть скорректированы"
type: docs
url: /ru/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Представляет, какие строки следует скорректировать.

```csharp
public enum AdjustFontSizeForRowType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без коррекции. |
| EmptyRows | `1` | Если строка пустая, измените размер шрифта, чтобы он соответствовал высоте строки. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните лист некоторыми данными
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Создайте экземпляр PptxSaveOptions с настройкой AdjustFontSizeForRowType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // Сохраните книгу в виде файла PPTX
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


