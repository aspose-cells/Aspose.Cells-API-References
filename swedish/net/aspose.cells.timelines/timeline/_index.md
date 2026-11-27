---
title: "Klass Timeline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Timelines.Timeline class. Sammanfattande beskrivning av Timeline-vyn På grund av att MS Excel Excel 2003 inte stöder Timeline"
type: docs
url: /sv/net/aspose.cells.timelines/timeline/
---
## Timeline class

Sammanfattande beskrivning av Timeline‑vyn. På grund av MS Excel stöder inte Excel 2003 Timeline.

```csharp
public class Timeline
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Hämtar eller anger rubriken för denna Timeline. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | Den aktuella tidsnivån för Timeline. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Hämtar eller anger höjden på den angivna tidslinjen, i pixlar. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Hämtar eller anger den horisontella förskjutningen av tidslinjeformen från dess vänstra kolumn, i pixlar. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Hämtar eller anger namnet på den angivna Timeline |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | Hämtar och anger tidsnivån där den aktuella markeringen gjordes för Timeline. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Hämtar [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) objektet som är associerat med denna Timeline. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | Anger om rubriken för denna tidslinje ska visas. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | Anger om den horisontella rullningslisten ska visas. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | Anger om urvalsetiketten ska visas. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | Anger om rullgardinsmenyn för tidsnivån ska visas. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | Hämtar och anger startdatumet för tidsintervallens rullningsposition för denna `Timeline`. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) Hämtar eller anger den vertikala förskjutningen av tidslinjeformen från dess översta rad, i pixlar. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) Hämtar eller anger bredden på den angivna tidslinjen, i pixlar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | Hämtar det valda datum‑tidsintervallet. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | Välj objekt mellan datum‑tiden. |

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i kalkylbladet med exempeldata
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Skapa datumformat
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Ange datumformat
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Lägg till en pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Uppdatera pivottabellens data
            pivot.RefreshData();
            pivot.CalculateData();

            // Lägg till en ny tidslinje med pivottabell som datakälla
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // Hämta tidslinjeobjekt
            Timeline timelineObj = sheet.Timelines[0];

            // Ange egenskaper för tidslinjen
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Spara arbetsboken
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


