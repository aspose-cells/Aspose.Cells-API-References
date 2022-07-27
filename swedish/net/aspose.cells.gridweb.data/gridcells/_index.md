---
title: GridCells
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in en samling avCell objekt.
type: docs
weight: 190
url: /sv/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Kapslar in en samling avCell objekt.

```csharp
public class GridCells : IEnumerable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.gridweb.data/gridcells/count) { get; } | Hämtar antalet celler. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.gridweb.data/gridcells/item) { get; } | BlirCell objekt i kalkylbladet (3 indexers) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn) { get; } | Maximalt kolumnindex för cell som innehåller data eller stil. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow) { get; } | Maximalt radindex för cell som innehåller data eller stil. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells) { get; } | Hämtar samlingen av sammanslagna celler. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator) { get; } | Hämtar radenumerator |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows) { get; } |  |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i poängenhet. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i pixelenhet. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth) { get; set; } | Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i teckenenhet. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels) { get; set; } |  |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear)() | Rensa alla celler i samlingen. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents)(GridCellArea) | Rensar innehållet i ett intervall. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | Rensar innehållet i ett intervall. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats)(GridCellArea) | Rensar formatering av ett intervall. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | Rensar formatering av ett intervall. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange)(GridCellArea) | Rensar innehåll och formatering av ett intervall. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | Rensar innehåll och formatering av ett intervall. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn)(GridCells, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns)(GridCells, int, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow)(GridCells, int, int) | Kopierar data och formatering av en hel rad. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows)(GridCells, int, int, int) | Kopierar data och formatering av vissa hela rader. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns)() | Ta bort alla tomma kolumner som inte innehåller några data. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows)() | Ta bort alla tomma rader som inte innehåller några data. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn)(int) | Tar bort en kolumn. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | Tar bort en kolumn. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns)(int, int, bool) | Tar bort flera kolumner. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange)(int, int, int, int, GridShiftType) | Tar bort ett intervall av celler och skiftar celler enligt skiftalternativet. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow)(int) | Tar bort en rad. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows)(int, int) | Tar bort flera rader. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows_1)(int, int, bool) | Tar bort flera rader i kalkylbladet. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export)(int, int, int, int, bool, bool) | Exporterar data i Cells-samlingen i ett WebWorksheet till ett nytt DataTable-objekt |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray)(int, int, int, int) | Exporterar data iCellssamling till ett tvådimensionellt arrayobjekt. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell)(int, int) | FårCell element eller null vid angivet cellradindex och kolumnindex. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth)(int) | Hämtar bredden på den angivna kolumnen |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch)(int) | Hämtar bredden på den angivna kolumnen, i enheter av tum. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel)(int) | Hämtar bredden på den angivna kolumnen, i enheter av pixlar. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator)() | Hämtar radenumerator |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow)(int) | FårRow element eller vid angivet cellradsindex. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight)(int) | Får höjden på en angiven rad. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch)(int) | Hämtar höjden på en angiven rad i enhet av tum. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel)(int) | Hämtar höjden på en angiven rad i pixelenhet. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel)(int) | Hämtar konturnivån för raden. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel)(int) | Få bredden i olika vytyper. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns)(int, int) | Grupper kolumner. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | Grupper kolumner. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows)(int, int) | Grupper rader. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn)(int) | Döljer en kolumn. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow)(int) | Döljer en rad. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn)(int) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns)(int, int) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | Infogar några kolumner i kalkylbladet. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange)(GridCellArea, GridShiftType) | Infogar ett område av celler och skift celler enligt skiftalternativet. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Infogar ett område av celler och skift celler enligt skiftalternativet. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow)(int) | Infogar en ny rad i kalkylbladet. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows)(int, int) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows_1)(int, int, bool) | Infogar flera rader i kalkylbladet. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn)(int) | Kontrollerar om given kolumn är tom (innehåller inga data). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden)(int) | Kontrollerar om en kolumn vid ett givet index är dold. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden)(int) | Kontrollerar om en rad vid ett givet index är dold. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge)(int, int, int, int) | Slår samman ett specificerat cellområde till en enda cell. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange)(GridCellArea, int, int) | Flyttar området. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas)() | Tar bort alla formler och ersätter med värdet på formeln. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Anger ramar för ett cellområde. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth)(int, double) | Anger bredden på den angivna kolumnen. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch)(int, double) | Ställer in kolumnbredden i tumenhet. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel)(int, int) | Ställer in kolumnbredden i pixelenhet. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight)(int, double) | Ställer in höjden på den angivna raden. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch)(int, double) | Ställer in radhöjden i tumenhet. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel)(int, int) | Ställer in radhöjden i pixelenhet. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel)(int, int) | Anger konturnivån för raden. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle_1)(string, GridTableItemStyle) | Ställer in stilen till ett specificerat cellintervall. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle)(int, int, int, int, GridTableItemStyle) | Ställer in stilen till ett specificerat cellintervall. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | Sorterar data stigande/nedåt uppifrån och ned i ett intervall i ett kalkylblad efter angivet kolumnindex. Sorterar uppgifterna stiger/sänker från vänster till höger i intervallet i ett kalkylblad efter angivet radindex. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns)(int, int) | Delar upp kolumner. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows)(int, int) | Delar upp rader. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn)(int, double) | Visar en kolumn |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow)(int) | Visar en rad. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge)(int, int, int, int) | Tar bort ett specificerat intervall av sammanslagna celler. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname)(int, int) | Hämtar cellnamn enligt dess rad- och kolumnindex. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex)(string, out int, out int) | Hämtar cellrads- och kolumnindex enligt dess namn |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname)(int) | Får kolumnnamn enligt kolumnindex. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex)(string) | Hämtar kolumnindex enligt kolumnnamn. |

### Se även

* namnutrymme [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* hopsättning [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
