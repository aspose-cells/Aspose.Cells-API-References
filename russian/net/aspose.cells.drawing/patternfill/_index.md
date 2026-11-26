---
title: "Класс PatternFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.PatternFill. Инкапсулирует объект, представляющий формат шаблонного заполнения."
type: docs
url: /ru/net/aspose.cells.drawing/patternfill/
---
## PatternFill class

Инкапсулирует объект, представляющий формат заполнения узором.

```csharp
public class PatternFill : Fill
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Получает и задает объект переднего [`CellsColor`](../../aspose.cells/cellscolor/). |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Получает или задает цвет фона [`Area`](../area/). |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Получает или задает прозрачность фонового цвета. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Получает и задает объект переднего [`CellsColor`](../../aspose.cells/cellscolor/). |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Получает или задает цвет переднего плана. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Получает или задает прозрачность переднего цвета. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Получает или задает тип шаблона заполнения. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Унаследовано от [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Получает хеш-код.(Унаследовано от [`Fill`](../fill/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassPatternFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль для ячейки, используя шаблон BackgroundType.
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.DiagonalStripe;
            style.ForegroundColor = Color.LightBlue;
            style.BackgroundColor = Color.DarkBlue;

            worksheet.Cells["B2"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("PatternFill Demo");

            // Создайте форму и настройте её заливку узором
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 100);
            shape.Fill.FillType = FillType.Pattern;
            
            PatternFill shapePatternFill = shape.Fill.PatternFill;
            shapePatternFill.Pattern = FillPattern.DiagonalBrick;
            shapePatternFill.ForegroundColor = Color.LightBlue;
            shapePatternFill.BackgroundColor = Color.DarkBlue;
            shapePatternFill.ForeTransparency = 0.2;
            shapePatternFill.BackTransparency = 0.3;

            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.Gold;
            shapePatternFill.ForegroundCellsColor = cellsColor;

            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


