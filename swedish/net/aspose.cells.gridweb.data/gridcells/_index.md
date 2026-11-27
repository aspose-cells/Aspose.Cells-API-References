---
title: "Klass GridCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridCells-klass. Inkapslar en samling av GridCell-objekt."
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Inkapslar en samling av [`GridCell`](../gridcell/) objekt.

```csharp
public class GridCells : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | Hämtar samlingen av [`GridColumn`](../gridcolumn/) objekt som representerar de enskilda kolumnerna i detta kalkylblad. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | Hämtar antalet celler. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | Hämtar den första cellen i detta kalkylblad. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | Hämtar [`GridCell`](../gridcell/)‑elementet på det angivna cellradindexet och kolumnindexet. (2 indexerare) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | Hämtar den sista cellen i detta kalkylblad. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | Maximalt kolumnindex för cell som innehåller data eller stil. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | Maximalt kolumnindex för celler som innehåller data. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | Maximalt radindex för celler som innehåller data. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | Maximalt radindex för celler som innehåller data eller stil. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | Hämtar samlingen av sammanslagna celler. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | Minsta kolumnindex för cellen som innehåller data. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | Minsta radindex för cellen som innehåller data. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | Minsta radindex för cellen som innehåller data eller stil. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | Hämtar radernas enumerator |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | Hämtar samlingen av [`GridRow`](../gridrow/)‑objekt som representerar de enskilda raderna i detta kalkylblad. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | Hämtar eller anger standardradhöjden i detta kalkylblad, i enheten punkter. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | Hämtar eller anger standardradhöjden i detta kalkylblad, i enheten pixlar. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tecken. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tum. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten pixlar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | Hämtar [`GridCell`](../gridcell/)‑elementet eller null vid det angivna cellradindexet och kolumnindexet. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | Hämtar [`GridColumn`](../gridcolumn/) elementet eller null på det angivna kolumnindexet. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | Hämtar [`GridRow`](../gridrow/)‑elementet eller null vid det angivna cellradindexet. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | Rensa alla celler i samlingen. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Rensar innehållet i ett område. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Rensar innehållet i ett område. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | Rensar formatering av ett område. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Rensar formatering av ett område. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | Rensar innehåll och formatering av ett område. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Rensar innehåll och formatering av ett område. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | Kopierar data och formatering av en hel rad. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | Kopierar data och formatering av några hela rader. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | Ta bort alla tomma rader som inte innehåller någon data. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | Tar bort en kolumn. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Tar bort en kolumn. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | Tar bort flera kolumner. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | Tar bort ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | Tar bort en rad. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | Tar bort flera rader. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Tar bort flera rader i kalkylbladet. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | Exporterar data i Cells-samlingen för ett WebWorksheet till ett nytt DataTable-objekt |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | Exporterar data i `GridCells`-samlingen till ett tvådimensionellt array-objekt. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | Hämtar [`GridCell`](../gridcell/) elementet på det angivna cellradindexet och kolumnindexet. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | Hämtar bredden på den angivna kolumnen |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | Hämtar bredden på den angivna kolumnen, i enheten tum. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | Hämtar bredden på den angivna kolumnen, i enheten pixel. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | Hämtar radernas enumerator |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | Hämtar [`GridRow`](../gridrow/)‑elementet eller vid det angivna cellradindexet. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | Hämtar höjden på en specificerad rad. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | Hämtar höjden på en specificerad rad i enhet tum. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | Hämtar höjden på en specificerad rad i enhet pixel. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | Hämtar konturnivån för raden. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | Hämta bredden i olika vystyper. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Grupperar kolumner. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Grupperar kolumner. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | Grupperar rader. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | Döljer en kolumn. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | Döljer en rad. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Infogar några kolumner i kalkylbladet. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | Infogar en ny rad i kalkylbladet. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Infogar flera rader i kalkylbladet. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | Kontrollerar om given kolumn är tom (innehåller ingen data). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | Kontrollerar om en kolumn på angivet index är dold. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | Kontrollerar om en rad på angivet index är dold. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | Slår ihop ett angivet cellområde till en enda cell. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | Flyttar området. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | Ta bort dubblettvärden i intervallet. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | Tar bort alla formler och ersätter dem med formelns värde. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Ställer in kanter för ett cellintervall. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | Anger bredden på den angivna kolumnen. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | Anger kolumnbredd i enheten tum. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | Anger kolumnbredd i enheten pixlar. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | Ställer in höjden på den angivna raden. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | Ställer in radens höjd i enhet tum. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | Ställer in radens höjd i enhet pixlar. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | Ställer in konturnivån för raden. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | Anger stilen för ett angivet cellområde. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | Anger stilen för ett angivet cellområde. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Sorterar data stigande/avtagande uppifrån och ner i ett område i ett kalkylblad efter angivet kolumnindex. Sorterar data stigande/avtagande vänster till höger i ett område i ett kalkylblad efter angivet radindex. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Sorterar data stigande/avtagande uppifrån och ner i ett område i ett kalkylblad efter angivet kolumnindex. Sorterar data stigande/avtagande vänster till höger i ett område i ett kalkylblad efter angivet radindex. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | Avgrupperar kolumner. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | Avgrupperar rader. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | Visar en dold kolumn |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | Visar en dold rad. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | Delar upp ett angivet område av sammanslagna celler. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | Hämtar cellnamn enligt dess rad- och kolumnindex. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | Hämtar cellens rad- och kolumnindex enligt dess namn |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | Hämtar kolumnnamn enligt kolumnindex. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | Hämtar kolumnindex enligt kolumnnamn. |

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


