---
title: "TwoColorGradient.Color1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TwoColorGradient. Получает и задает первый цвет градиента"
type: docs
url: /ru/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

Получает и устанавливает первый цвет градиента.

```csharp
public Color Color1 { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Создайте стиль с заливкой градиентом
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // Инициализируйте двухцветный градиент
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // Примените градиент к стилю ячейки
            cell.SetStyle(style);
            
            // Прочитайте начальный цвет
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // Измените цвет градиента и примените снова
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // Проверьте обновление
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // Визуальная демонстрация в выходном файле
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### См. также

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


