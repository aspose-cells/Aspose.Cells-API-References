---
title: "Класс PivotArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotArea. Представляет выбранную область сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

Отображает выбранную область сводной таблицы.

```csharp
public class PivotArea
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | Представляет выбранную область сводной таблицы. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Получает и задает область сводной таблицы, к которой применяется это правило. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Получает все фильтры для этой области PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Указывает, включён ли общий итог по столбцу. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Указывает, относится ли правило к области, находящейся в режиме структуры. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Указывает, включен ли общий итог строки. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Указывает, выбираются ли только значения данных (в области данных представления) для выбранного элемента и не включают ли метки элементов. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Указывает, выбираются ли только метки данных для выбранного элемента. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Получает и задает тип правила выбора. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Получает области ячеек этого сводного диапазона. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Выберите область с фильтрами. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Выберите поле в регионе в качестве области. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Выберите поле в регионе в качестве области. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Добавьте сводную таблицу на лист.
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Создайте экземпляр PivotArea.
            PivotArea pivotArea = new PivotArea(pivotTable);

            // Установите свойства PivotArea.
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Используйте метод Select для выбора конкретной области.
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Сохраните книгу
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


