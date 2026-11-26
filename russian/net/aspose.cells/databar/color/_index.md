---
title: "DataBar.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Получить или установить цвет этой DataBar"
type: docs
url: /ru/net/aspose.cells/databar/color/
---
## DataBar.Color property

Получить или установить цвет этого DataBar.

```csharp
public Color Color { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон ячеек
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Добавьте некоторые образцы данных.
            worksheet.Cells["E3"].PutValue(10);
            worksheet.Cells["F3"].PutValue(20);
            worksheet.Cells["G3"].PutValue(30);
            worksheet.Cells["E4"].PutValue(15);
            worksheet.Cells["F4"].PutValue(25);
            worksheet.Cells["G4"].PutValue(35);

            // Добавьте условное форматирование с полосой данных
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Установите свойства полосы данных, включая Color
            condition.DataBar.Color = Color.Orange;
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            condition.DataBar.ShowValue = false;

            // Установить свойства границы
            condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            condition.DataBar.BarBorder.Color = Color.Plum;

            // Установить тип заливки
            condition.DataBar.BarFillType = DataBarFillType.Gradient;

            // Установить свойства оси
            condition.DataBar.AxisColor = Color.Red;
            condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;

            // Установите свойства отрицательной полосы
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Примените форматирование к диапазону
            conditions.AddArea(area);

            // Сохраните книгу
            workbook.Save("DataBarPropertyColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBarPropertyColorDemo executed successfully.");
        }
    }
}
```

### См. также

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


