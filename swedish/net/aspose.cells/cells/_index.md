---
title: "Klassen Cells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Cells-klass. Inkapslar en samling av cellrelaterade objekt såsom Cell, Row …etc"
type: docs
url: /sv/net/aspose.cells/cells/
---
## Cells class

Inkapslar en samling av cellrelaterade objekt, såsom [`Cell`](../cell/), [`Row`](../row/), …etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | Hämtar samlingen av [`Column`](../column/)-objekt som representerar de enskilda kolumnerna i detta kalkylblad. |
| [Count](../../aspose.cells/cells/count/) { get; } | Hämtar det totala antalet instansierade Cell-objekt. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | Hämtar det totala antalet instansierade Cell-objekt. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | Hämtar den första cellen i detta kalkylblad. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | Indikerar att radhöjd och standardteckensnittshöjd matchar |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | Indikerar om raden är standarddolt. |
| [Item](../../aspose.cells/cells/item/) { get; } | Hämtar [`Cell`](../cell/)-elementet på det angivna cellradindexet och kolumnindexet. (2 indexerare) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | Hämtar den sista cellen i detta kalkylblad. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | Maximalt kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | Maximalt kolumnindex för celler som innehåller data. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | Maximalt radindex för celler som innehåller data. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | Hämtar det maximala området som inkluderar data, sammanslagna celler och former. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | Maximalt radindex för celler som innehåller data eller stil. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | Hämtar eller anger minnesanvändningsalternativet för dessa celler. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsolete.**) Hämtar samlingen av sammanslagna celler. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | Minsta kolumnindex för cellen som innehåller data. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | Minsta radindex för cellen som innehåller data. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | Minsta radindex för cellen som innehåller data eller stil. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | Hämtar eller anger om cellernas datamodell ska stödja Multi-Thread läsning. Standardvärdet för denna egenskap är falskt. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | Hämtar listan över fält i ods. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | Hämtar eller anger ett värde som indikerar om alla kalkylbladsvärden bevaras som strängar. Standard är falskt. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | Hämtar samlingen av [`Range`](../range/) objekt som skapas vid körning. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | Hämtar samlingen av [`Row`](../row/) objekt som representerar de enskilda raderna i detta kalkylblad. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | Hämtar eller anger standardradshöjden i detta kalkylblad, i enheten punkter. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | Hämtar eller anger standardradshöjden i detta kalkylblad, i enheten tum. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | Hämtar eller anger standardradshöjden i detta kalkylblad, i enheten pixlar. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tecken. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten tum. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten pixlar. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | Hämtar och anger standardstilen för kalkylbladet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | Lägger till en referens till ett områdeobjekt i celler. |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | Tillämpar format för en hel kolumn. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | Tillämpar format för en hel rad. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | Tillämpar format för ett helt kalkylblad. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | Hämtar [`Cell`](../cell/)-elementet eller null på det angivna cellradindexet och kolumnindexet. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | Hämtar [`Column`](../column/)-elementet eller null på det angivna kolumnindexet. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | Hämtar [`Row`](../row/)-elementet eller null på det angivna cellradindexet. |
| [Clear](../../aspose.cells/cells/clear/)() | Rensar all data i kalkylbladet. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | Rensar innehållet i ett område. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | Rensar innehållet i ett område. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | Rensar formatering av ett område. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | Rensar formatering av ett område. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | Rensar alla sammanslagna områden. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | Rensar innehåll och formatering av ett område. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | Rensar innehåll och formatering av ett område. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | Konverterar all strängdata i kalkylbladet till numeriskt värde om möjligt. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | Kopierar data och format för en hel kolumn. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | Kopierar data och format för hela kolumner. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | Kopierar data och format för de hela kolumnerna. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | Kopierar data och format för en hel kolumn. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | Kopierar data och format för en hel rad. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | Kopierar data och format för några hela rader. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | Kopierar data och format för några hela rader. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Kopierar data och format för några hela rader. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | Skapar ett [`Range`](../range/)‑objekt från en adress för området. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | Skapar ett [`Range`](../range/) objekt från ett område av celler. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | Skapar ett [`Range`](../range/) objekt från rader av celler eller kolumner av celler. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | Skapar ett [`Range`](../range/) objekt från ett område av celler. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | Ta bort alla tomma rader som inte innehåller någon data eller annat objekt. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | Ta bort alla tomma rader som inte innehåller någon data eller vissa speciella objekt såsom synlig kommentar, pivottabell. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | Tar bort en kolumn. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | Tar bort en kolumn. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | Tar bort flera kolumner. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | Tar bort flera kolumner. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | Tar bort ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | Tar bort en rad. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | Tar bort en rad. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | Tar bort flera rader. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | Tar bort flera rader i kalkylbladet. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | Tar bort flera rader i kalkylbladet. |
| [Dispose](../../aspose.cells/cells/dispose/)() | Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | Hämtar den sista cellen i den här kolumnen. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | Hämtar den sista cellen med högsta kolumnindex i detta område. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | Hämtar den sista cellen i den här raden. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | Hämtar den sista cellen med högsta radindex i detta område. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | Exporterar data i `Cells`‑samlingen till ett tvådimensionellt array‑objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | Exporterar data i `Cells`-samlingen till ett DataTable-objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | Exporterar data i `Cells`-samlingen till ett DataTable-objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exporterar data i `Cells`-samlingen till ett DataTable-objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | Exporterar data i `Cells`-samlingen till ett DataTable-objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | Exporterar data i `Cells`-samlingen till ett DataTable-objekt. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | Exporterar cellvärdestyp i `Cells`-samlingen till ett tvådimensionellt array-objekt. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | Hittar cellen som innehåller det angivna objektet. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | Hittar cellen som innehåller det angivna objektet. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsolete.**) Hämtar [`Cell`](../cell/) elementet eller null vid det angivna cellradindexet och kolumnindexet. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | Hämta visningsstilen för given cell. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | Hämta visningsstilen för given cell. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | Hämta stilen för given cell. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | Hämtar alla celler som innehåller inbäddad bild. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsolete.**) Hämtar kolumnens ursprungliga höjd i punktenheter om kolumnen är dold |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | Hämtar bredden (i tecken) för den angivna kolumnen i normal vy |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | Hämtar kolumnbredden. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsolete.**) Hämtar bredden för den angivna kolumnen i normal vy, i tum. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | Hämtar bredden för den angivna kolumnen i normal vy, i pixlar. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsolete.**) Hämtar bredden för den angivna kolumnen i normal vy, i pixlar. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | Hämta alla celler som refererar till den specifika cellen. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | Hämtar alla celler vars beräknade resultat beror på en specifik cell. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | Hämtar cellernas enumerator. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | Hämtar det första radindexet för cellen som innehåller data i den angivna kolumnen. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | Hämtar konturnivån (nollbaserad) för kolumnen. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | Hämtar konturnivån (nollbaserad) för raden. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | Hämtar det sista radindexet för cellen som innehåller data i den angivna kolumnen. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | Hämtar den maximala grupperade kolumnens konturnivå (nollbaserad). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | Hämtar den maximala grupperade radens konturnivå (nollbaserad). |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | Hämtar alla sammanslagna celler. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsolete.**) Hämtar [`Row`](../row/) elementet vid det angivna cellradindexet. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsolete.**) Hämtar radernas enumerator. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | Hämtar höjden på en specificerad rad, i enhet punkter. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | Hämtar radens höjd. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | Hämtar höjden på en specificerad rad i enhet tum. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | Hämtar höjden på en specificerad rad i enhet pixel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) Hämtar originalradens höjd i enhet punkt om raden är dold |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | Hämta bredden i olika vystyper. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | Hämtar höjden på en specificerad rad. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | Hämtar höjden på en specificerad rad i enhet tum. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | Grupperar kolumner. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | Grupperar kolumner. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | Grupperar rader. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | Grupperar rader. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | Döljer en kolumn. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | Dölj flera kolumner. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | Komprimerar de grupperade raderna/kolumnerna. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | Döljer en rad. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | Döljer flera rader. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | Importerar en array av double till ett kalkylblad. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | Importerar en array av integer till ett kalkylblad. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | Importerar en array av string till ett kalkylblad. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | Importerar en arraylist av data till ett kalkylblad. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importerar anpassade objekt. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importerar anpassade objekt. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | Importerar data från ett IDataReader-objekt. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | Importera data från en anpassad datatabell. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | Importera data från en datavy. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importera data från en anpassad datatabell. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importerar data från ett IDataReader-objekt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | Importerar en DataGrid till ett kalkylblad. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importerar en DataGrid till ett kalkylblad. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importerar en DataGrid till ett kalkylblad. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | Importerar en DataGrid till ett kalkylblad. Denna metod försöker inte konvertera text till numeriska värden. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | Importerar en DataRow till Excel-filen. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | Importerar en DataView till ett kalkylblad. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | Importerar en matris av formler till ett kalkylblad. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | Importerar en rutnätsvy till dessa celler. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | Importerar en matris av data till ett kalkylblad. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | Importerar en matris av data till ett kalkylblad. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | Infogar några kolumner i kalkylbladet. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | Infoga klippt område. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | Infogar ett cellområde och flyttar celler enligt förskjutningsalternativet. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | Infogar en ny rad i kalkylbladet. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | Infogar flera rader i kalkylbladet. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | Kontrollerar om given kolumn är tom (innehåller ingen data). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | Kontrollerar om en kolumn på angivet index är dold. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | Kontrollera om området kan tas bort. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | Kontrollerar om en rad på angivet index är dold. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | Länk till en XML-karta. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | Slår ihop ett angivet cellområde till en enda cell. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | Slår ihop ett angivet cellområde till en enda cell. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | Slår ihop ett angivet cellområde till en enda cell. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | Flyttar området. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | Tar bort dubblett-rader i bladet. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | Tar bort dubblettvärden i området. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | Tar bort dubblettdata i området. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | Tar bort alla formler och ersätter dem med formelns värde. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | Hämtar subtotalinställningarna för området. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | Ställer in bredden på den angivna kolumnen i normal vy. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | Ställer in kolumnbredd i tum i normal vy. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | Ställer in kolumnbredd i enhet pixlar i normal vy. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | Ställer in höjden på den angivna raden. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | Ställer in radens höjd i enhet tum. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | Ställer in radens höjd i enhet pixlar. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | Ställer in kolumnens bredd i olika vyer. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | Expanderar de grupperade raderna/kolumnerna. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Skapar delsummer för intervallet. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Skapar delsummer för intervallet. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | Delar upp innehållet i angiven kolumn i flera kolumner.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | Avgrupperar kolumner. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | Avgrupperar rader. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | Avgrupperar rader. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | Visar en dold kolumn |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | Visa flera dolda kolumner. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | Visar en dold rad. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | Visar de dolda raderna. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | Delar upp ett angivet område av sammanslagna celler. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in standardradshöjd
            cells.StandardHeight = 20;
            // Ställ in radens höjd
            cells.SetRowHeight(2, 20.5);

            // Ställ in standardkolumnbredd
            cells.StandardWidth = 15;
            // Ställ in kolumnbredd
            cells.SetColumnWidth(3, 12.57);

            // Sammanfoga celler
            cells.Merge(5, 4, 2, 2);

            // Sätt värden i celler
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // Exportera data
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Demonstrera några egenskaper
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // Iterera genom celler
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Spara arbetsboken
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


