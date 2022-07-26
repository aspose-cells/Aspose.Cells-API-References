---
title: GridCells
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in en samling avCellobjekt.
type: docs
weight: 410
url: /sv/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Kapslar in en samling avCellobjekt.

```csharp
public class GridCells : IEnumerable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count) { get; } | Hämtar antalet celler. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item) { get; } | BlirCell objekt i kalkylbladet (3 indexers) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn) { get; } | Maximalt kolumnindex för cell som innehåller data eller stil. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow) { get; } | Maximalt radindex för cell som innehåller data eller stil. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells) { get; } | Hämtar samlingen av sammanslagna celler. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator) { get; } | Hämtar radenumerator |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows) { get; } | Får samlingen av[`GridRow`](../gridrow) objekt som representerar de individuella raderna i detta kalkylblad. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i poängenhet. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i pixelenhet. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth) { get; set; } | Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i teckenenhet. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels) { get; set; } |  |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell)(int, int) | FårCell element eller null vid angivet cellradindex och kolumnindex. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear)() | Rensa alla celler i samlingen. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents)(GridCellArea) | Rensar innehållet i ett intervall. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | Rensar innehållet i ett intervall. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats)(GridCellArea) | Rensar formatering av ett intervall. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | Rensar formatering av ett intervall. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange)(GridCellArea) | Rensar innehåll och formatering av ett intervall. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | Rensar innehåll och formatering av ett intervall. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn)(GridCells, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns)(GridCells, int, int, int) | Kopierar data och formatering av en hel kolumn. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow)(GridCells, int, int) | Kopierar data och formatering av en hel rad. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows)(GridCells, int, int, int) | Kopierar data och formatering av vissa hela rader. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns)() | Ta bort alla tomma kolumner som inte innehåller några data. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows)() | Ta bort alla tomma rader som inte innehåller några data. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn)(int) | Tar bort en kolumn. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | Tar bort en kolumn. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns)(int, int, bool) | Tar bort flera kolumner. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow)(int) | Tar bort en rad. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows)(int, int) | Tar bort flera rader. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows_1)(int, int, bool) | Tar bort flera rader i kalkylbladet. |
| [GetCell](../../aspose.cells.griddesktop.data/gridcells/getcell)(int, int) | FårCell element eller null vid angivet cellradindex och kolumnindex. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle)(int, int) | Få stilen för given cell. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn)(int) | Får[`GridColumn`](../gridcolumn) element eller vid angivet cellkolumnindex. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth)(int) | Hämtar bredden på den angivna kolumnen |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch)(int) | Hämtar bredden på den angivna kolumnen, i enheter av tum. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel)(int) | Hämtar bredden på den angivna kolumnen, i enheter av pixlar. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator)() | Hämtar radenumerator |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow)(int) | Får[`GridRow`](../gridrow) element eller vid angivet cellradsindex. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight)(int) | Får höjden på en angiven rad. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch)(int) | Hämtar höjden på en angiven rad i enhet av tum. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel)(int) | Hämtar höjden på en angiven rad i pixelenhet. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel)(int) | Få bredden i olika vytyper. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns)(int, int) | Grupper kolumner. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | Grupper kolumner. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows)(int, int) | Grupper rader. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn)(int) | Döljer en kolumn. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow)(int) | Döljer en rad. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn)(int) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns)(int, int) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | Infogar några kolumner i kalkylbladet. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow)(int) | Infogar en ny rad i kalkylbladet. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows)(int, int) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows_1)(int, int, bool) | Infogar flera rader i kalkylbladet. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn)(int) | Kontrollerar om given kolumn är tom (innehåller inga data). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden)(int) | Kontrollerar om en kolumn vid ett givet index är dold. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden)(int) | Kontrollerar om en rad vid ett givet index är dold. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge)(int, int, int, int) | Slår samman ett specificerat cellområde till en enda cell. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas)() | Tar bort alla formler och ersätter med värdet på formeln. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth)(int, double) | Anger bredden på den angivna kolumnen. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch)(int, double) | Ställer in kolumnbredden i tumenhet. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel)(int, int) | Ställer in kolumnbredden i pixelenhet. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight)(int, double) | Ställer in höjden på den angivna raden. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch)(int, double) | Ställer in radhöjden i tumenhet. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel)(int, int) | Ställer in radhöjden i pixelenhet. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle)(CellRange, Style) | Ställer in stilen till ett specificerat cellintervall. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_2)(string, Style) | Ställer in stilen till ett specificerat cellintervall. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_1)(int, int, int, int, Style) | Ställer in stilen till ett specificerat cellintervall. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | Sorterar data stigande/nedåt uppifrån och ned i ett intervall i ett kalkylblad efter angivet kolumnindex. Sorterar uppgifterna stiger/sänker från vänster till höger i intervallet i ett kalkylblad efter angivet radindex. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns)(int, int) | Delar upp kolumner. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows)(int, int) | Delar upp rader. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn)(int, double) | Visar en kolumn |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow)(int) | Visar en rad. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge)(int, int, int, int) | Tar bort ett specificerat intervall av sammanslagna celler. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname)(int, int) | Hämtar cellnamn enligt dess rad- och kolumnindex. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex)(string, out int, out int) | Hämtar cellrads- och kolumnindex enligt dess namn |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname)(int) | Får kolumnnamn enligt kolumnindex. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex)(string) | Hämtar kolumnindex enligt kolumnnamn. |

### Se även

* namnutrymme [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* hopsättning [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
