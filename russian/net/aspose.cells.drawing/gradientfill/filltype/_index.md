---
title: "GradientFill.FillType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GradientFill. Возвращает тип заполнения градиентом"
type: docs
url: /ru/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Получает тип градиентной заливки.

```csharp
public GradientFillType FillType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму с градиентным заполнением
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // Установить свойства градиента
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Отобразить тип градиентного заполнения
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // Изменить на радиальный градиент
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // Сохраните книгу
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### См. также

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


