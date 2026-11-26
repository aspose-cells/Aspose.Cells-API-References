---
title: "BorderCollection.DiagonalStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BorderCollection. Получает или задаёт стиль диагональных линий"
type: docs
url: /ru/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Получает или задает style диагональных линий.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить ячейку и её стиль
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Установить свойства диагональной границы
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // Применить стиль к ячейке
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


