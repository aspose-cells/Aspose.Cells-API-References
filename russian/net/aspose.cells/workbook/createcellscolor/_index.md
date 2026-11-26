---
title: "Workbook.CreateCellsColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Создает объект CellsColor"
type: docs
url: /ru/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Создает объект [`CellsColor`](../../cellscolor/).

```csharp
public CellsColor CreateCellsColor()
```

### Возвращаемое значение

Возвращает объект [`CellsColor`](../../cellscolor/).

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Создайте диапазон и установите границы с пользовательским цветом
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // Проверьте стиль границы в конкретной ячейке
            Cell cell = workbook.Worksheets[0].Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);

            workbook.Save("CreateCellsColorExample.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


