---
title: "CellsColor.IsShapeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsColor. Получает и задает цвет, который должен применяться к ячейке или форме"
type: docs
url: /ru/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Получает и задает цвет, который должен применяться к ячейке или фигуре.

```csharp
public bool IsShapeColor { get; set; }
```

### Примечания

Выражение цвета ячейки и формы различается. Например, цвет темы с тем же значением оттенка будет отличаться в ячейке и форме.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyIsShapeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр CellsColor и установите IsShapeColor
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // Примените цвет к форме
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // Сохраните книгу
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


