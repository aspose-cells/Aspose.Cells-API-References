---
title: "TwoColorGradient.Color2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TwoColorGradient. Получает и задает второй цвет градиента"
type: docs
url: /ru/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

Получает и устанавливает второй цвет градиента.

```csharp
public Color Color2 { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр двухцветного градиента
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // Создайте первый стиль с начальным градиентом
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // Отобразите текущее значение Color2
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // Измените свойство Color2
            gradient.Color2 = Color.Red;

            // Создайте второй стиль с изменённым градиентом
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // Отрегулируйте строки для видимости
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // Сохраните книгу
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### См. также

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


