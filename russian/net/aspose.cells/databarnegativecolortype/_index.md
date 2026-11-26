---
title: "Перечисление DataBarNegativeColorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DataBarNegativeColorType. Указывает, использовать ли тот же цвет границы и заливки, что и у положительных полос данных"
type: docs
url: /ru/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

Указывает, использовать ли тот же цвет границы и заливки, что и у положительных гистограмм.

```csharp
public enum DataBarNegativeColorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Color | `0` | Использовать цвет, указанный в диалоговом окне Negative Value and Axis Setting, или с помощью свойств ColorType и BorderColorType объекта NegativeBarFormat. |
| SameAsPositive | `1` | Использовать тот же цвет, что и у положительных полос данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Установить свойства полос данных
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Установить свойства формата отрицательной полосы
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Сохраните книгу
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


