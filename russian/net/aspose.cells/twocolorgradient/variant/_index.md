---
title: "TwoColorGradient.Variant"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TwoColorGradient. Получает и устанавливает вариант градиента"
type: docs
url: /ru/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

Получает и устанавливает вариант градиента.

```csharp
public int Variant { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте двухцветный градиент с начальным вариантом
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // Создайте и примените стиль к ячейке A1
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // Отобразите текущее значение варианта
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // Измените значение варианта
            gradient.Variant = 2;

            // Создайте и примените изменённый стиль к ячейке B1
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // Увеличьте высоту ячеек, чтобы визуализировать градиенты
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### См. также

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


