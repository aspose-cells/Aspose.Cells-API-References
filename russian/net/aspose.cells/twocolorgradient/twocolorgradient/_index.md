---
title: "TwoColorGradient.TwoColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор TwoColorGradient."
type: docs
url: /ru/net/aspose.cells/twocolorgradient/twocolorgradient/
---
## TwoColorGradient constructor

```csharp
public TwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| color1 | Color |  |
| color2 | Color |  |
| gradientStyleType | GradientStyleType |  |
| variant | Int32 |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class TwoColorGradientMethodSharpctorWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр TwoColorGradient, используя конструктор со всеми параметрами
                TwoColorGradient gradient = new TwoColorGradient(
                    Color.LightBlue,
                    Color.DarkBlue,
                    GradientStyleType.Horizontal,
                    1);

                // Отобразите свойства градиента, чтобы проверить инициализацию
                Console.WriteLine($"Gradient created with:");
                Console.WriteLine($"Color1: {gradient.Color1}");
                Console.WriteLine($"Color2: {gradient.Color2}");
                Console.WriteLine($"GradientStyleType: {gradient.GradientStyleType}");
                Console.WriteLine($"Variant: {gradient.Variant}");

                // Создайте книгу и примените градиент, чтобы продемонстрировать функциональность
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Примените градиент к ячейке
                Style style = workbook.CreateStyle();
                style.SetTwoColorGradient(
                    gradient.Color1,
                    gradient.Color2,
                    gradient.GradientStyleType,
                    gradient.Variant);

                worksheet.Cells["A1"].PutValue("TwoColorGradient Demo");
                worksheet.Cells["A1"].SetStyle(style);

                // Сохраните книгу
                workbook.Save("TwoColorGradientDemo.xlsx");
                Console.WriteLine("Gradient applied successfully to workbook.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


