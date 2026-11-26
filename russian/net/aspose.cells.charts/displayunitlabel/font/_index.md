---
title: "DisplayUnitLabel.Font"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DisplayUnitLabel. Возвращает объект Font указанного объекта ChartFrame"
type: docs
url: /ru/net/aspose.cells.charts/displayunitlabel/font/
---
## DisplayUnitLabel.Font property

Возвращает объект `Font` указанного объекта ChartFrame.

```csharp
public override Font Font { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitLabelPropertyFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            worksheet.Cells["A5"].PutValue(5000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Установить единицы отображения для оси значений
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.DisplayUnitLabel.Text = "Thousands";

            // Получить экземпляр DisplayUnitLabel
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Отобразить текущие свойства шрифта
            Font currentFont = displayUnitLabel.Font;
            Console.WriteLine("Current Font Properties:");
            Console.WriteLine($"Name: {currentFont.Name}");
            Console.WriteLine($"Size: {currentFont.Size}");
            Console.WriteLine($"Color: {currentFont.Color}");
            Console.WriteLine($"Bold: {currentFont.IsBold}");
            Console.WriteLine($"Italic: {currentFont.IsItalic}");

            // Создать новый стиль шрифта и применить его к DisplayUnitLabel
            // Примечание: Поскольку Font только для чтения, мы изменяем его свойства напрямую
            currentFont.Name = "Arial";
            currentFont.Size = 12;
            currentFont.Color = System.Drawing.Color.Red;
            currentFont.IsBold = true;
            currentFont.IsItalic = false;
            currentFont.Underline = FontUnderlineType.Single;

            // Сохраните рабочую книгу, чтобы увидеть изменения
            workbook.Save("DisplayUnitLabelFontDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../../../aspose.cells/font/)
* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


