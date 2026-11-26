---
title: "Класс AboveAverage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AboveAverage. Описывает правило условного форматирования AboveAverage. Это правило условного форматирования выделяет ячейки, значения которых находятся выше или ниже среднего для всех значений в диапазоне."
type: docs
url: /ru/net/aspose.cells/aboveaverage/
---
## AboveAverage class

Опишите правило условного форматирования AboveAverage. Это правило условного форматирования выделяет ячейки, значения которых выше или ниже среднего для всех значений в диапазоне.

```csharp
public class AboveAverage
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AboveAverage](aboveaverage/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Получить или задать флаг, указывающий, является ли правило правилом "above average". Значение 'true' означает "above average". Значение по умолчанию — true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | Получить или задать флаг, указывающий, включают ли критерии 'aboveAverage' и 'belowAverage' само среднее значение или исключают его. Значение 'true' означает включить среднее значение в критерий. Значение по умолчанию — false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Получить или задать количество стандартных отклонений, включаемых выше или ниже среднего в правиле условного форматирования. Входное значение должно быть от 0 до 3 (включительно). Установка значения 0 означает, что stdDev не задан. Значение по умолчанию — 0. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            // Добавить коллекцию условного форматирования в лист
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Определить область ячеек для применения условного форматирования
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Добавить условие above average в коллекцию
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Установить цвет фона для условия
            fc.Style.BackgroundColor = Color.Yellow;

            // Установить свойства для условия above average
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // Сохраните книгу
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


