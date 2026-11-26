---
title: "FillFormat.SolidFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Возвращает объект SolidFill"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Возвращает объект `SolidFill`.

```csharp
public SolidFill SolidFill { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertySolidFillDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Установите цвет сплошного заполнения для фигуры
            shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
            
            // Получите и отобразите цвет сплошного заполнения
            System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
            Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}", 
                fillColor.R, fillColor.G, fillColor.B);
            
            // Сохраните книгу
            workbook.Save("SolidFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


