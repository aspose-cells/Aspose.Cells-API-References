---
title: "Класс ColorScale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ColorScale. Описание правила условного форматирования ColorScale. Это правило условного форматирования создает градиентную цветовую шкалу в ячейках"
type: docs
url: /ru/net/aspose.cells/colorscale/
---
## ColorScale class

Опишите правило условного форматирования ColorScale. Это правило условного форматирования создает градиентную цветовую шкалу в ячейках.

```csharp
public class ColorScale
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Указывает, является ли условное форматирование трехцветной шкалой. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Получить или установить объект максимального значения этого ColorScale. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Получить или установить градиентный цвет для максимального значения в диапазоне. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Получить или установить объект среднего значения этого ColorScale. Нельзя установить CFValueObject с типом FormatConditionValueType.Max или FormatConditionValueType.Min. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Получить или установить градиентный цвет для среднего значения в диапазоне. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Получить или установить объект минимального значения этого ColorScale. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Получить или установить градиентный цвет для минимального значения в диапазоне. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Добавить правило условного форматирования
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Получить доступ к объекту ColorScale
            ColorScale colorScale = fc.ColorScale;

            // Установить свойства для ColorScale
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Установить объекты минимального, среднего и максимального значений
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // Сохраните книгу
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


