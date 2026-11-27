---
title: "Klass GridCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.Data.GridCells klass. Inkapslar en samling av Cell-objekt"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Inkapslar en samling av Cell-objekt.

```csharp
public class GridCells : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | Hämtar antalet celler. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | Hämtar den första cellen i detta kalkylblad. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | Hämtar [`GridCell`](../gridcell/)‑elementet på det angivna cellradindexet och kolumnindexet. (2 indexerare) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | Hämtar den sista cellen i detta kalkylblad. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | Maximalt kolumnindex för cell som innehåller data eller stil. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | Maximalt kolumnindex för celler som innehåller data. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | Maximalt radindex för celler som innehåller data. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | Maximalt radindex för celler som innehåller data eller stil. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | Hämtar samlingen av sammanslagna celler. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | Minsta kolumnindex för cellen som innehåller data. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | Minsta radindex för cellen som innehåller data. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | Minsta radindex för cellen som innehåller data eller stil. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | Hämtar radernas enumerator |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | Hämtar samlingen av [`GridRow`](../gridrow/)‑objekt som representerar de enskilda raderna i detta kalkylblad. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | Hämtar eller anger standardradhöjden i detta kalkylblad, i enheten punkter. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | Hämtar eller anger standardradhöjden i detta kalkylblad, i enheten pixlar. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tecken. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | Hämtar [`GridCell`](../gridcell/)‑elementet eller null vid det angivna cellradindexet och kolumnindexet. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | Hämtar [`GridRow`](../gridrow/)‑elementet eller null vid det angivna cellradindexet. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | Rensa alla celler i samlingen. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Rensar innehållet i ett område. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Rensar innehållet i ett område. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | Rensar formatering av ett område. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Rensar formatering av ett område. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | Rensar innehåll och formatering av ett område. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Rensar innehåll och formatering av ett område. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | Kopierar data och formatering av en hel rad. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | Kopierar data och formatering av några hela rader. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | Ta bort alla tomma rader som inte innehåller någon data. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | Tar bort en kolumn. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Tar bort en kolumn. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | Tar bort flera kolumner. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | Tar bort en rad. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | Tar bort flera rader. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Tar bort flera rader i kalkylbladet. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | Hämta stilen för given cell. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | Hämtar [`GridColumn`](../gridcolumn/)‑elementet eller vid det angivna cellkolumnindexet. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | Hämtar bredden på den angivna kolumnen |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | Hämtar bredden på den angivna kolumnen, i enheten tum. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | Hämtar bredden på den angivna kolumnen, i enheten pixel. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | Hämtar radernas enumerator |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | Hämtar [`GridRow`](../gridrow/)‑elementet eller vid det angivna cellradindexet. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | Hämtar höjden på en specificerad rad. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | Hämtar höjden på en specificerad rad i enhet tum. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | Hämtar höjden på en specificerad rad i enhet pixel. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | Hämta bredden i olika vystyper. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Grupperar kolumner. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Grupperar kolumner. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | Grupperar rader. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | Döljer en kolumn. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | Dölj flera kolumner. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | Döljer en rad. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | Döljer flera rader. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Infogar några kolumner i kalkylbladet. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | Infogar en ny rad i kalkylbladet. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Infogar flera rader i kalkylbladet. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | Kontrollerar om given kolumn är tom (innehåller ingen data). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | Kontrollerar om en kolumn på angivet index är dold. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | Kontrollerar om en rad på angivet index är dold. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | Slår ihop ett angivet cellområde till en enda cell. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | Tar bort alla formler och ersätter dem med formelns värde. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | Anger bredden på den angivna kolumnen. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | Anger kolumnbredd i enheten tum. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | Anger kolumnbredd i enheten pixlar. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | Ställer in höjden på den angivna raden. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | Ställer in radens höjd i enhet tum. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | Ställer in radens höjd i enhet pixlar. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | Anger stilen för ett angivet cellområde. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | Anger stilen för ett angivet cellområde. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | Anger stilen för ett angivet cellområde. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Sorterar data stigande/avtagande uppifrån och ner i ett område i ett kalkylblad efter angivet kolumnindex. Sorterar data stigande/avtagande vänster till höger i ett område i ett kalkylblad efter angivet radindex. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | Sorterar data i området. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | Sorterar data i området (nyckelkolumnens data ska vara ett tal). |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | Avgrupperar kolumner. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | Avgrupperar rader. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | Visar en dold kolumn |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | Visa flera dolda kolumner. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | Visar en dold rad. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | Visar de dolda raderna. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | Delar upp ett angivet område av sammanslagna celler. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | Hämtar cellnamn enligt dess rad- och kolumnindex. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | Hämtar cellens rad- och kolumnindex enligt dess namn |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | Hämtar kolumnnamn enligt kolumnindex. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | Hämtar kolumnindex enligt kolumnnamn. |

### Se även

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


