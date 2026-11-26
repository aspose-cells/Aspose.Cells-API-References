---
title: "Перечисление DataBarFillType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DataBarFillType. Указывает, как заполняется полоса данных цветом"
type: docs
url: /ru/net/aspose.cells/databarfilltype/
---
## DataBarFillType enumeration

Указывает, как гистограмма заполняется цветом.

```csharp
public enum DataBarFillType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Solid | `0` | Полоса данных заполнена сплошным цветом. |
| Gradient | `1` | Полоса данных заполнена градиентом цвета. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarFillTypeDemo
    {
        public static void DataBarFillTypeExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Добавление нового листа в Workbook
            Worksheet sheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Добавляет условие
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Получить Databar
            DataBar dataBar = cond.DataBar;

            // Установить свойства Databar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Задать значения ячеек
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Сохранение файла Excel
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


