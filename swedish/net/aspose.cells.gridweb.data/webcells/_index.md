---
title: "Klass WebCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.WebCells-klass."
type: docs
url: /sv/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Hämtar antalet celler. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Hämtar Cell‑elementet vid det angivna cellradindexet och kolumnindexet. (2 indexerare) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Hämtar samlingen av sammanslagna celler. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Minsta kolumnnummer för cell som innehåller data eller stil. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Minsta radnummer för cell som innehåller data eller stil. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Hämtar eller anger standardradhöjden i detta kalkylblad, i enheten punkter. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tecken. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Rensar innehållet i ett område. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Tar bort en kolumn. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Tar bort en rad. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Tar bort ett antal rader. Denna metod är mycket snabbare än DeleteRow vid batchraderade. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Exporterar data i Cells-samlingen för ett WebWorksheet till ett nytt DataTable-objekt |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Exporterar data i Cells-samlingen till ett tvådimensionellt array‑objekt. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Hämtar kolumnrubriken. Om rubriken inte är angiven returneras en tom sträng. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Hämtar om en kolumn är skrivskyddad. Detta är en utökad metod i GridWeb specifikt, den kommer inte att sparas eller påverka den faktiska Excel-filen. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Hämtar bredden på den angivna kolumnen |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Hämtar cellernas enumerator |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Hämtar radrubriken. Om rubriken inte är angiven returneras en tom sträng. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Hämtar höjden på en specificerad rad. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Hämta dold status för en specificerad rad. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Hämtar konturnivån för raden. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Hämtar om en rad är skrivskyddad. Detta är en utökad metod i GridWeb specifikt, den kommer inte att sparas eller påverka den faktiska Excel-filen. |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Infogar en ny kolumn i kalkylbladet. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Infogar en ny rad i kalkylbladet. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Infogar flera rader i kalkylbladet. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Ställer in kanter för ett cellintervall. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Ställer in rubriken för kolumnen. Observera att detta är ett extensionsattribut och inte kan sparas i Excel-filen. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Ställer in en kolumn som skrivskyddad så att användaren inte kan ta bort den från klientsidan. Detta är en utökad metod för GridWeb specifikt, den kommer inte att sparas eller ha effekt i den faktiska Excel-filen. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Ställer in bredden på den specificerade kolumnen. Den accepterade breddtypen är Point, Pixel eller Inch. |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Ställer in rubriken för raden. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Ställer in höjden på den specificerade raden. Den accepterade breddtypen är Point, Pixel eller Inch. |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Ställ in dold status för en specificerad rad. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Ställer in konturnivån för raden. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Ställer in konturnivån för raden. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Ställer in en rad som skrivskyddad så att användaren inte kan ta bort den från klientsidan. Detta är en utökad metod för GridWeb specifikt, den kommer inte att sparas eller ha effekt i den faktiska Excel-filen. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Anger stilen för ett angivet cellområde. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Anger stilen för ett angivet cellområde. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | Sorterar data stigande uppifrån och ner i ett område av ett WebWorksheet efter specificerat kolumnindex. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | Sorterar data stigande uppifrån och ner i ett område av ett WebWorksheet efter några fält som specificeras av en array med kolumnindex. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | Sorterar data stigande uppifrån och ner i ett område av ett WebWorksheet efter specificerat kolumnindex. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Sorterar data stigande i ett område av ett WebWorksheet efter några fält som specificeras av en indexarray. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Delar upp ett angivet område av sammanslagna celler. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Hämtar cellnamn enligt dess rad- och kolumnindex. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Hämtar cellens rad- och kolumnindex enligt dess namn |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Hämtar kolumnnamn enligt kolumnindex. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Hämtar kolumnindex enligt kolumnnamn. |

### Anmärkningar

OBS: Denna klass är nu föråldrad. vänligen använd GridCells istället. Denna klass kommer att tas bort efter 6 månader från augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


