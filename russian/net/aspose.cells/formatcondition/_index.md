---
title: "Класс FormatCondition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FormatCondition. Представляет условие условного форматирования"
type: docs
url: /ru/net/aspose.cells/formatcondition/
---
## FormatCondition class

Представляет условие условного форматирования.

```csharp
public class FormatCondition
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | Получить экземпляр "AboveAverage" условного форматирования. Правило экземпляра по умолчанию выделяет ячейки, значения которых выше среднего для всех значений в диапазоне. Действительно только для type = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | Получить экземпляр "ColorScale" условного форматирования. Экземпляр по умолчанию представляет собой "green-yellow-red" 3ColorScale. Действительно только для type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | Получить экземпляр "DataBar" условного форматирования. Цвет экземпляра по умолчанию — синий. Действительно только для type = DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | Получает и задает значение или выражение, связанное с условным форматированием. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | Получает и задает значение или выражение, связанное с условным форматированием. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | Получить экземпляр "IconSet" условного форматирования. IconSetType экземпляра по умолчанию — TrafficLights31. Действительно только для type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | Получает и задает тип оператора условного формата. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | Приоритет этого правила условного форматирования. Это значение используется для определения, какой формат следует оценивать и применять. Меньшие числовые значения имеют более высокий приоритет, чем большие, где '1' — высший приоритет. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | True, правила с более низким приоритетом не могут применяться к этому правилу, когда оно оценивается как true. Применяется только к Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | Получает или задает стиль диапазонов ячеек, условно отформатированных. |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | Текстовое значение в правиле условного форматирования "text contains". Действительно только для type = containsText, notContainsText, beginsWith и endsWith. Значение по умолчанию — null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | Применимый период времени в правиле условного форматирования "date occurrin". Действительно только для type = timePeriod. Значение по умолчанию — TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | Получить экземпляр "Top10" условного форматирования. Правило экземпляра по умолчанию выделяет ячейки, значения которых находятся в топ‑10. Действительно только для type = Top10. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | Получает и задает, включен ли тип условного формата. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | Получает значение или выражение, связанное с этим условием формата. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | Получает формулу условного форматирования ячейки. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | Получает значение или выражение условного форматирования ячейки. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | Получает значение или выражение, связанное с этим условием формата. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | Получает формулу условного форматирования ячейки. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | Получает значение или выражение условного форматирования ячейки. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | Задает значение или выражение, связанное с этим условием формата. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | Задает значение или выражение, связанное с этим условием формата. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | Задает значение или выражение, связанное с этим условием формата. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionDemo
    {
        public static void FormatConditionExample()
        {
            // Создайте новую Workbook.
            Workbook workbook = new Workbook();

            // Получите первый worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Добавляет условие.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // Установка свойств
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // Демонстрация других свойств
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // Сохранение файла Excel
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


