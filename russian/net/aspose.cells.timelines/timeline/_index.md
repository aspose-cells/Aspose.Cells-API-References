---
title: "Класс Timeline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Timelines.Timeline. Краткое описание представления Timeline. Из‑за того, что MS Excel 2003 не поддерживает Timeline"
type: docs
url: /ru/net/aspose.cells.timelines/timeline/
---
## Timeline class

Краткое описание представления Timeline. Из‑за MS Excel, Excel 2003 не поддерживает Timeline.

```csharp
public class Timeline
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Получает или задаёт подпись этого Timeline. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | Текущий уровень времени Timeline. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Возвращает или задаёт высоту указанного timeline в пикселях. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Возвращает или задаёт горизонтальное смещение формы timeline от её левого столбца в пикселях. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Возвращает или задаёт имя указанного Timeline |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | Получает и задаёт уровень времени, на котором была сделана текущая выборка для Timeline. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Возвращает объект [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) , связанный с этим Timeline. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | Указывает, следует ли отображать заголовок этого timeline. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | Указывает, следует ли отображать горизонтальную полосу прокрутки. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | Указывает, следует ли отображать метку выбора. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | Указывает, следует ли отображать выпадающий список выбора уровня времени. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | Получает и задает дату начала позиции прокрутки временного интервала этого `Timeline`. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Устарело.**) Возвращает или задает вертикальное смещение формы временной шкалы от её верхней строки, в пикселях. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Устарело.**) Возвращает или задает ширину указанной временной шкалы, в пикселях. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | Получает выбранный диапазон даты и времени. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | Выберите элемент между датой и временем. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Timelines;
    using System;

    public class TimelineDemo
    {
        public static void TimelineExample()
        {
            // Создайте новую книгу и получите первый лист
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить лист образцовыми данными
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Создать стиль даты
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Установить стиль даты
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Добавить сводную таблицу
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Обновить данные сводной таблицы
            pivot.RefreshData();
            pivot.CalculateData();

            // Добавить новую временную шкалу, используя сводную таблицу в качестве источника данных
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // Получить объект Timeline
            Timeline timelineObj = sheet.Timelines[0];

            // Установить свойства Timeline
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Сохраните книгу
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


