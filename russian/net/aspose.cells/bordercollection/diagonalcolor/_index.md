---
title: "BorderCollection.DiagonalColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BorderCollection. Получает или задает цвет диагональных линий"
type: docs
url: /ru/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

Получает или задает Color диагональных линий.

```csharp
public Color DiagonalColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Border Demo");

            Style style = cell.GetStyle();
            
            // Настройка свойств диагональной границы
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


