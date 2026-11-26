---
title: "Структура CellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Структура Aspose.Cells.CellArea. Представляет область ячеек"
type: docs
url: /ru/net/aspose.cells/cellarea/
---
## CellArea structure

Представляет область ячеек.

```csharp
public struct CellArea : IComparable
```

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Создаёт область ячеек. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Создаёт область ячеек. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Сравнивает два объекта CellArea по их левому верхнему углу. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Возвращает строку, представляющую текущий объект области ячеек. |

## Поля

| Имя | Описание |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Получает или задаёт конечный столбец этой области. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Получает или задаёт конечную строку этой области. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Получает или задаёт начальный столбец этой области. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Получает или задаёт начальную строку этой области. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // Создать область ячеек
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Добавить правило условного форматирования в лист
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Сохраните книгу
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // Продемонстрировать метод ToString
            Console.WriteLine(ca.ToString());

            // Продемонстрировать метод CompareTo
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


