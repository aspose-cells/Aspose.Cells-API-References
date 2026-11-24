---
title: "Klasse AutoFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AutoFilter Klasse. Stellt die Autofilterung für das angegebene Arbeitsblatt dar"
type: docs
url: /de/net/aspose.cells/autofilter/
---
## AutoFilter class

Stellt die Autofilterung für das angegebene Arbeitsblatt dar.

```csharp
public class AutoFilter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Liest die Sammlung der Filterspalten. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Gibt an, ob die AutoFilter-Schaltfläche für diese Spalte sichtbar ist. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Liest den Datensortierer. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Fügt einen Datumsfilter hinzu. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Fügt einen Füllfarbenfilter hinzu. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Fügt einen Filter für eine Filterspalte hinzu. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Fügt einen Schriftfarbenfilter hinzu. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Fügt einen Symbolfilter hinzu. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Filtert eine Liste mit einem benutzerdefinierten Kriterium. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Filtert eine Liste mit benutzerdefinierten Kriterien. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Fügt einen dynamischen Filter hinzu. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Filtert eine Liste mit angegebenen Kriterien. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Filtere die obersten 10 Elemente in der Liste |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Liest den [`CellArea`](../cellarea/) aus, auf den dieser AutoFilter angewendet wird. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Liest den [`CellArea`](../cellarea/) aus, auf den der angegebene AutoFilter angewendet wird. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Alle leeren Zellen in der Liste abgleichen. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Alle nicht-leeren Zellen in der Liste abgleichen. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Aktualisiere AutoFilter, um Zeilen auszublenden oder wieder einzublenden. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Liest die Indizes aller ausgeblendeten Zeilen. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Entfernt einen Datumsfilter. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Entfernt den spezifischen Filter. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Entfernt einen Filter für eine Filterspalte. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Alle Zeilen einblenden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Erstelle einen Dateistream, der die zu öffnende Excel-Datei enthält
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Zugriff auf das erste Arbeitsblatt in der Excel-Datei
            Worksheet worksheet = workbook.Worksheets[0];
            // Erstelle AutoFilter, indem der Zellenbereich der Überschriftszeile angegeben wird
            worksheet.AutoFilter.Range = "A1:B8";
            // Filtern von Spalten mit angegebenen Werten
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Speichern der modifizierten Excel-Datei.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Instanziieren eines Workbook-Objekts
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Zugriff auf das erste Arbeitsblatt in der Excel-Datei
            worksheet = workbook.Worksheets[0];

            // Zusätzlicher Code, um weitere Funktionen von AutoFilter zu demonstrieren
            // Festlegen des Bereichs für AutoFilter
            worksheet.AutoFilter.Range = "A1:B8";
            // Hinzufügen eines Filters
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Hinzufügen eines Datumsfilters
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Speichern der modifizierten Excel-Datei.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Instanziieren eines Workbook-Objekts
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Zugriff auf das erste Arbeitsblatt in der Excel-Datei
            worksheet = workbook.Worksheets[0];
                        
            // Hinzufügen eines Schriftfarbenfilters
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Speichern der modifizierten Excel-Datei.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Instanziieren eines Workbook-Objekts
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Zugriff auf das erste Arbeitsblatt in der Excel-Datei
            worksheet = workbook.Worksheets[0];

            // Hinzufügen eines Füllfarbenfilters
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Speichern der modifizierten Excel-Datei.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Instanziieren eines Workbook-Objekts
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Zugriff auf das erste Arbeitsblatt in der Excel-Datei
            worksheet = workbook.Worksheets[0];

            // Übereinstimmung leerer Zellen
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Speichern der modifizierten Excel-Datei.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Instanziieren eines Workbook-Objekts
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Zugriff auf das erste Arbeitsblatt in der Excel-Datei
            worksheet = workbook.Worksheets[0];

            // Übereinstimmung nicht-leerer Zellen
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Speichern der modifizierten Excel-Datei.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Instanziieren eines Workbook-Objekts
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Zugriff auf das erste Arbeitsblatt in der Excel-Datei
            worksheet = workbook.Worksheets[0];

            // Benutzerdefinierter Filter
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Speichern der modifizierten Excel-Datei.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


