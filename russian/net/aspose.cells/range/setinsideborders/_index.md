---
title: "Range.SetInsideBorders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Устанавливает внутренние границы диапазона"
type: docs
url: /ru/net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Устанавливает внутренние границы диапазона.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| borderEdge | BorderType | Тип внутренней границы, может быть только вертикальной или горизонтальной. |
| lineStyle | CellBorderType | Стиль границы. |
| borderColor | CellsColor | Цвет границы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetInsideBordersWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте диапазон и установите внутренние границы
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);

            // Проверьте границы в ячейке внутри диапазона
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            workbook.Save("SetInsideBordersExample.xlsx");
        }
    }
}
```

### См. также

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


