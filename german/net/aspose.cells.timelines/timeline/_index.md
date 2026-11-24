---
title: "Klasse Timeline"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Timelines.Timeline Klasse. Zusammenfassende Beschreibung der Timeline-Ansicht, da MS Excel 2003 die Timeline nicht unterstützt"
type: docs
url: /de/net/aspose.cells.timelines/timeline/
---
## Timeline class

Zusammenfassende Beschreibung der Timeline-Ansicht. Aufgrund von MS Excel unterstützt Excel 2003 keine Timeline.

```csharp
public class Timeline
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Liest oder setzt die Beschriftung dieser Timeline. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | Die aktuelle Zeitebene der Timeline. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Gibt die Höhe der angegebenen Timeline zurück oder legt sie fest, in Pixeln. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Gibt den horizontalen Versatz der Timeline-Form von ihrer linken Spalte zurück oder legt ihn fest, in Pixeln. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Gibt den Namen der angegebenen Timeline zurück oder legt ihn fest |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | Liest und setzt die Zeitebene, auf der die aktuelle Auswahl für die Timeline getroffen wurde. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Gibt das [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) Objekt zurück, das mit dieser Timeline verknüpft ist. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | Gibt an, ob die Kopfzeile dieser Timeline angezeigt werden soll. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | Gibt an, ob die horizontale Bildlaufleiste angezeigt werden soll. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | Gibt an, ob das Auswahl-Label angezeigt werden soll. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | Gibt an, ob das Dropdown-Auswahlfeld der Zeitebene angezeigt werden soll. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | Liest und setzt das Startdatum der Bildlaufposition des Zeitraums dieser `Timeline`. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) Gibt den vertikalen Versatz der Timeline-Form von ihrer oberen Zeile zurück oder legt ihn fest, in Pixeln. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) Gibt die Breite der angegebenen Timeline zurück oder legt sie fest, in Pixeln. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | Liest den ausgewählten Datums-Zeit-Bereich. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | Element zwischen den Datum-Zeit-Werten auswählen. |

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Arbeitsblatt mit Beispieldaten füllen
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Datumsformat erstellen
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Datumsformat festlegen
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Füge eine PivotTable hinzu
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // PivotTable-Daten aktualisieren
            pivot.RefreshData();
            pivot.CalculateData();

            // Füge eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // Timeline-Objekt abrufen
            Timeline timelineObj = sheet.Timelines[0];

            // Eigenschaften der Timeline festlegen
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Speichere die Arbeitsmappe
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


