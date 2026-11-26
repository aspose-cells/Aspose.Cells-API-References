---
title: "Перечисление PresetWordArtStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.PresetWordArtStyle перечисление. Представляет предустановленные стили WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

Представляет предустановленные стили WordArt.

```csharp
public enum PresetWordArtStyle
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| WordArtStyle1 | `1` | Заполнение - Черный, Текст 1, Тень |
| WordArtStyle2 | `2` | Заполнение - Синий, Акцент 1, Тень |
| WordArtStyle3 | `3` | Заполнение - Оранжевый, Акцент 2, Контур - Акцент 2 |
| WordArtStyle4 | `4` | Заполнение - Белый, Контур - Акцент 1, Тень |
| WordArtStyle5 | `5` | Заполнение - Золотой, Акцент 4, Мягкая фаска |
| WordArtStyle6 | `6` | Градиентное заполнение - Серый |
| WordArtStyle7 | `7` | Градиентное заполнение - Синий, Акцент 1, Отражение |
| WordArtStyle8 | `8` | Градиентное заполнение - Золотой, Акцент 4, Контур - Акцент 4 |
| WordArtStyle9 | `9` | Заполнение - Белый, Контур - Акцент 1, Свечение - Акцент 1 |
| WordArtStyle10 | `10` | Заполнение - Серый-50%, Акцент 3, Острая фаска |
| WordArtStyle11 | `11` | Заливка - Чёрный, Текст 1, Обводка - Фон 1, Жёсткая тень - Фон 1 |
| WordArtStyle12 | `12` | Заливка - Чёрный, Текст 1, Обводка - Фон 1, Жёсткая тень - Акцент 1 |
| WordArtStyle13 | `13` | Заливка - Синий, Акцент 1, Обводка - Фон 1, Жёсткая тень - Акцент 1 |
| WordArtStyle14 | `14` | Заливка - Белый, Обводка - Акцент 2, Жёсткая тень - Акцент 2 |
| WordArtStyle15 | `15` | Заливка - Серый-25%, Фон 2, Внутренняя тень |
| WordArtStyle16 | `16` | Заполнение узором - Белый, Текст 2, Тёмная восходящая диагональ, Тень |
| WordArtStyle17 | `17` | Заполнение узором - Серый-50%, Акцент 3, Узкая горизонтальная, Внутренняя тень |
| WordArtStyle18 | `18` | Заливка - Синий, Акцент 1, 50%, Жёсткая тень - Акцент 1 |
| WordArtStyle19 | `19` | Заполнение узором - Синий, Акцент 1, Светлая нисходящая диагональ, Обводка - Акцент 1 |
| WordArtStyle20 | `20` | Заполнение узором - Сине-серый, Текст 2, Тёмная восходящая диагональ, Жёсткая тень - Текст 2 |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PresetWordArtStyleDemo
    {
        public static void PresetWordArtStyleExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к коллекции фигур листа
            ShapeCollection shapes = worksheet.Shapes;
            
            // Добавить форму WordArt с определённым предустановленным стилем
            // Параметры: style, text, upperLeftRow, top, upperLeftColumn, left, height, width
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // Сохраните книгу
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


