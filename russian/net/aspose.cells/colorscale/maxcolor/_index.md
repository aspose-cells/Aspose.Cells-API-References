---
title: "ColorScale.MaxColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ColorScale. Получить или установить градиентный цвет для максимального значения в диапазоне"
type: docs
url: /ru/net/aspose.cells/colorscale/maxcolor/
---
## ColorScale.MaxColor property

Получить или установить градиентный цвет для максимального значения в диапазоне.

```csharp
public Color MaxColor { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxColorDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Создать объект CellArea вместо использования строки
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Добавить условие цветовой шкалы
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];
            ColorScale colorScale = fc.ColorScale;

            // Настроить цветовую шкалу
            colorScale.Is3ColorScale = false; // Use 2-color scale for simplicity
            colorScale.MinColor = Color.Green;
            colorScale.MaxColor = Color.Red; // Demonstrating MaxColor property

            // Установить объекты значений
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Сохраните книгу
            workbook.Save("ColorScaleMaxColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


