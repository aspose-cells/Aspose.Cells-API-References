---
title: "Worksheet.Shapes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает все графические фигуры в этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Возвращает все графические фигуры в этом листе.

```csharp
public ShapeCollection Shapes { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShapesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте несколько фигур в лист
            sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
            
            // Измените свойства фигур
            for (int i = 0; i < sheet.Shapes.Count; i++)
            {
                Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
                Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
                
                // Обновите свойства первой фигуры
                if (i == 0)
                {
                    shape.Name = "MyRectangle";
                    shape.FillFormat.ForeColor = System.Drawing.Color.Red;
                }
            }
            
            // Сохраните книгу
            workbook.Save("ShapesDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


