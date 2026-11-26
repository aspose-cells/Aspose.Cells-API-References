---
title: "Класс NegativeBarFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.NegativeBarFormat. Представляет настройки цвета полос данных для отрицательных значений, определённых правилом условного форматирования полос данных"
type: docs
url: /ru/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

Представляет настройки цвета полос данных для отрицательных значений, определённых правилом условного форматирования полос данных.

```csharp
public class NegativeBarFormat
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Получает или задает объект FormatColor, который можно использовать для указания цвета границы отрицательных полос данных. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Указывает, следует ли использовать тот же цвет границы, что и у положительных полос данных. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Получает или задает объект FormatColor, который можно использовать для указания цвета заливки отрицательных полос данных. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Получает или задает, следует ли использовать тот же цвет заливки, что и у положительных полос данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // Создайте объект Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Добавляет условие для DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Получите DataBar и задайте его свойства
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Настройте свойства NegativeBarFormat
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Поместите некоторые значения в ячейки
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Сохраните книгу
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


