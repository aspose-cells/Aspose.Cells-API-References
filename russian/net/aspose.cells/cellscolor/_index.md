---
title: "Класс CellsColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellsColor. Представляет все типы цветов"
type: docs
url: /ru/net/aspose.cells/cellscolor/
---
## CellsColor class

Представляет все типы цветов.

```csharp
public class CellsColor
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | Получает и задает цвет из 32‑битного значения ARGB. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | Получает и задает цвет RGB. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Получает и задает индекс цвета в палитре. Применяется только для индексированных цветов. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Получает и задает цвет, который должен применяться к ячейке или фигуре. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Получает цвет темы. Применяется только к типу цвета темы. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Получает и задает прозрачность в диапазоне от 0,0 (непрозрачный) до 1,0 (прозрачный). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | Тип цвета. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Установить оттенок цвета фигуры |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон ячеек
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Создать экземпляр CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Установить свойства CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // Применить CellsColor к диапазону
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Сохраните книгу
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


