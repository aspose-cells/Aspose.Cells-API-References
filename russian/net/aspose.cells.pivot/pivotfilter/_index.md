---
title: "Класс PivotFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotFilter. Представляет PivotFilter в коллекции PivotFilter"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Представляет PivotFilter в коллекции PivotFilter.

```csharp
public class PivotFilter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) Получает автофильтр сводного фильтра. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Получает порядок оценки сводного фильтра. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Получает индекс исходного поля, к которому применяется этот сводный фильтр. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Получает категорию этого фильтра. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Получает тип фильтра сводного фильтра. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Указывает индекс поля измерения куба. Это свойство используется только фильтрами в OLAP pivots и определяет, к какому измерению следует применять фильтр значений. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) Получает индекс поля измерения сводного фильтра. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Получает индекс поля свойства члена сводного фильтра. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Получает имя сводного фильтра. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Указывает, использовать ли полные дни в критериях фильтрации по дате. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Получает строковое значение value1 метки сводного фильтра. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Получает строковое значение value2 метки сводного фильтра. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Получает индекс поля значения в области значений. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Получает значения числового фильтра. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Получает метки фильтра подписи. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Получает значения числового фильтра. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Получает настройку топ‑10 фильтра. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // Создать новую книгу
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить лист образцовыми данными
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Добавьте сводную таблицу на лист.
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Установить стиль pivot table
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Добавить сводный фильтр
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Установить дополнительные свойства для сводного фильтра
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Обновить и вычислить данные сводной таблицы
            pivot.RefreshData();
            pivot.CalculateData();

            // Сохраните книгу
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


