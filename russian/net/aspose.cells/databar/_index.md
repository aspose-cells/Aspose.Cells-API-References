---
title: "Класс DataBar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DataBar. Описывает правило условного форматирования DataBar. Это правило условного форматирования отображает градиентную полосу данных в диапазоне ячеек"
type: docs
url: /ru/net/aspose.cells/databar/
---
## DataBar class

Опишите правило условного форматирования DataBar. Это правило условного форматирования отображает градиентную полосу данных в диапазоне ячеек.

```csharp
public class DataBar
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Получает цвет оси для ячеек с условным форматированием в виде полос данных. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Получает или задает положение оси полос данных, указанное правилом условного форматирования. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Получает объект, определяющий границу полосы данных. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Получает или задает способ заполнения полосы данных цветом. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Получить или установить цвет этого DataBar. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | Получает или задает направление отображения databar. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Получить или установить объект максимального значения этого DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Представляет максимальную длину data bar. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Получить или установить объект минимального значения этого DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Представляет минимальную длину data bar. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Получает объект NegativeBarFormat, связанный с правилом условного форматирования data bar. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Получить или установить флаг, указывающий, показывать ли значения ячеек, к которым применён этот data bar. Значение по умолчанию — true. |

## Методы

| Имя | Описание |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Отрисовать data bar в ячейке в массив байтов изображения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Добавляет условие
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Получить DataBar
            DataBar dataBar = cond.DataBar;

            // Установить свойства DataBar
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
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // Сохранение файла Excel
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


