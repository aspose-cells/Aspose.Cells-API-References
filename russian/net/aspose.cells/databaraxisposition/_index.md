---
title: "Перечисление DataBarAxisPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DataBarAxisPosition. Указывает позицию оси для диапазона ячеек с условным форматированием в виде гистограмм"
type: docs
url: /ru/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

Указывает позицию оси для диапазона ячеек с условным форматированием в виде гистограмм.

```csharp
public enum DataBarAxisPosition
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Отображать ось в переменной позиции на основе отношения минимального отрицательного значения к максимальному положительному значению в диапазоне. Положительные значения отображаются слева направо. Отрицательные значения отображаются справа налево. Когда все значения положительные или все отрицательные, ось не отображается. |
| Midpoint | `1` | Отображать ось в середине ячейки независимо от набора значений в диапазоне. Положительные значения отображаются слева направо. Отрицательные значения отображаются справа налево. |
| None | `2` | Ось не отображается, а положительные и отрицательные значения отображаются слева направо. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarAxisPositionDemo
    {
        public static void DataBarAxisPositionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавление правила условного форматирования
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Установка диапазона условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Добавление условия гистограммы
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Установка свойств гистограммы
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // Установка значений ячеек
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // Сохранение файла Excel
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


