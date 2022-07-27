---
title: Cells
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in en samling cellrelevanta objekt som t.exCell./cell Row./row ...etc.
type: docs
weight: 300
url: /sv/net/aspose.cells/cells/
---
## Cells class

Kapslar in en samling cellrelevanta objekt, som t.ex[`Cell`](../cell) ,[`Row`](../row) ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | Får samlingen av[`Column`](../column) objekt som representerar de enskilda kolumnerna i detta kalkylblad. |
| [Count](../../aspose.cells/cells/count) { get; } | Får det totala antalet instansierade cellobjekt. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | Får det totala antalet instansierade cellobjekt. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | Hämtar den första cellen i detta kalkylblad. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | Indikerar att radhöjd och standardteckensnittshöjd matchar |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | Indikerar om raden är dold som standard. |
| [Item](../../aspose.cells/cells/item) { get; } | Får[`Cell`](../cell) element vid angivet cellradindex och kolumnindex. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | Hämtar den sista cellen i detta kalkylblad. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | Maximalt kolumnindex för cell som innehåller data. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | Maximalt radindex för cell som innehåller data. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | Hämtar det maximala intervallet som inkluderar data, sammanslagna celler och former. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | Maximalt radindex för cell som innehåller data eller stil. |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | Hämtar eller ställer in minnesanvändningsalternativet för denna cell. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | Hämtar samlingen av sammanslagna celler. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | Minsta kolumnindex för cell som innehåller data. |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | Minsta radindex för cell som innehåller data. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | Minsta radindex för cell som innehåller data eller stil. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | Hämtar eller ställer in om celldatamodellen ska stödja multitrådsläsning. Standardvärdet för den här egenskapen är false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | Hämtar listan över fält av ods. |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | Hämtar eller ställer in ett värde som anger om alla kalkylbladsvärden bevaras som strängar. Standard är falskt. |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | Får samlingen av[`Range`](../range)objekt skapade vid körning. |
| [Rows](../../aspose.cells/cells/rows) { get; } | Får samlingen av[`Row`](../row) objekt som representerar de individuella raderna i detta kalkylblad. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i poängenhet. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i tumenhet. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i pixelenhet. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i teckenenhet. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i enhet av tum. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i pixelenhet. |
| [Style](../../aspose.cells/cells/style) { get; set; } | Hämtar och ställer in standardstilen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | Lägger till en intervallobjektreferens till cells |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | Tillämpar format för en hel kolumn. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | Tillämpar format för en hel rad. |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | Tillämpar format för ett helt kalkylblad. |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | Får[`Cell`](../cell) element eller null vid angivet cellradindex och kolumnindex. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | Får[`Column`](../column) element eller null vid angivet kolumnindex. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | Får[`Row`](../row) element eller vid angivet cellradsindex. |
| [Clear](../../aspose.cells/cells/clear)() | Rensar alla cell- och radobjekt. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | Rensar innehållet i ett intervall. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | Rensar innehållet i ett intervall. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | Rensar formatering av ett intervall. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | Rensar formatering av ett intervall. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | Rensar alla sammanslagna intervall. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | Rensar innehåll och formatering av ett intervall. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | Rensar innehåll och formatering av ett intervall. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | Konverterar strängdata i celler till numeriskt värde om möjligt. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | Kopierar data och format för en hel kolumn. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | Kopierar data och format för en hel kolumn. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | Kopierar data och format för hela kolumnerna. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | Kopierar data och format för en hel kolumn. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | Kopierar data och format för en hel rad. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | Kopierar data och format för vissa hela rader. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | Kopierar data och format för vissa hela rader. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Kopierar data och format för vissa hela rader. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | Skapar en[`Range`](../range) objekt från en adress i området. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | Skapar en[`Range`](../range) objekt från ett cellintervall. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | Skapar en[`Range`](../range) objekt från rader med celler eller kolumner med celler. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | Skapar en[`Range`](../range) objekt från ett cellintervall. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | Ta bort alla tomma kolumner som inte innehåller några data. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | Ta bort alla tomma kolumner som inte innehåller några data. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | Ta bort alla tomma rader som inte innehåller några data. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | Ta bort alla tomma rader som inte innehåller några data. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | Tar bort en kolumn. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | Tar bort en kolumn. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | Tar bort flera kolumner. |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | Tar bort ett intervall av celler och skiftar celler enligt skiftalternativet. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | Tar bort en rad. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | Tar bort flera rader. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | Tar bort flera rader i kalkylbladet. |
| [Dispose](../../aspose.cells/cells/dispose)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | Hämtar den sista cellen i denna kolumn. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | Hämtar den sista cellen med maximalt kolumnindex i detta intervall. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | Hämtar den sista cellen i den här raden. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | Hämtar den sista cellen med maximalt radindex i detta intervall. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | Exporterar data i[`Cells`](../cells) samling till ett tvådimensionellt arrayobjekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | Exporterar data i[`Cells`](../cells) samling till enDataTable objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | Exporterar data i[`Cells`](../cells) samling till enDataTable objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exporterar data i[`Cells`](../cells) samling till enDataTable objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | Exporterar data i[`Cells`](../cells) samling till enDataTable objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | Exporterar data i[`Cells`](../cells) samling till enDataTable objekt. |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | Exporterar cellvärdestyp i[`Cells`](../cells) samling till ett tvådimensionellt arrayobjekt. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | Hittar cellen som innehåller med indataobjektet. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | Hittar cellen som innehåller med indataobjektet. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | Får[`Cell`](../cell) element eller null vid angivet cellradindex och kolumnindex. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | Få stilen för given cell. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | Hämtar bredden på den angivna kolumnen i normal view |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | Hämtar bredden på den angivna kolumnen i normalvy, i enheter av tum. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | Hämtar bredden på den angivna kolumnen i normal vy, i enheter av pixlar. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | Hämta alla celler som refererar till den specifika cellen. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | Hämtar alla celler vars beräknade resultat beror på specifik cell. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | Hämtar celluppräkningen. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | Hämtar konturnivån (nollbaserad) för kolumnen. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | Får konturnivån (nollbaserad) för raden. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | Hämtar den sista radens index i cellen som innehåller data i den angivna kolumnen. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | Får den maximala grupperade kolumnkonturnivån (nollbaserad). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | Får den maximala grupperade radkonturnivån (nollbaserad). |
| [GetRow](../../aspose.cells/cells/getrow)(int) | Får[`Row`](../row) element vid angivet cellradsindex. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | Hämtar raduppräkningen. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | Får höjden på en angiven rad. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | Hämtar höjden på en angiven rad i enhet av tum. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | Hämtar höjden på en angiven rad i pixelenhet. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | Får den ursprungliga radens höjd i punktenhet om raden är dold |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | Få bredden i olika vytyper. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | Får höjden på en angiven rad. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | Hämtar höjden på en angiven rad i enhet av tum. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | Grupper kolumner. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | Grupper kolumner. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | Grupper rader. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | Grupper rader. |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | Döljer en kolumn. |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | Dölj flera kolumner. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | Komprimerar de grupperade raderna/kolumnerna. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | Döljer en rad. |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | Döljer flera rader. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | Importerar en array av dubbel till ett kalkylblad. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | Importerar en matris med heltal till ett kalkylblad. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | Importerar en array av sträng till ett kalkylblad. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | Importerar en arraylista med data till ett kalkylblad. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | Importera en CSV-fil till cellerna. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importerar anpassade objekt. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importerar anpassade objekt. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | Importerar data från enIDataReader objekt. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | Importera data från anpassad datatabell. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | Importera data från datavyn. |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importera data från anpassad datatabell. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importerar data från enIDataReader objekt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | Importer aDataGrid i ett kalkylblad. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importer aDataGrid i ett kalkylblad. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importer aDataGrid i ett kalkylblad. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | Importer aDataGrid i ett arbetsblad. Den här metoden försöker inte konvertera text till numeriska värden. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | Importerar en DataRow till Excel-filen. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | Importer aDataView i ett kalkylblad. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | Importerar en matris med formel till ett kalkylblad. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | Importerar en rutnätsvy till dessa celler. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | Importerar en mängd data till ett kalkylblad. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | Importerar en mängd data till ett kalkylblad. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | Infogar några kolumner i kalkylbladet. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | Insert cut range. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | Infogar ett område av celler och skift celler enligt skiftalternativet. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | Infogar ett område av celler och skift celler enligt skiftalternativet. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | Infogar ett område av celler och skift celler enligt skiftalternativet. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | Infogar en ny rad i kalkylbladet. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | Infogar flera rader i kalkylbladet. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | Infogar flera rader i kalkylbladet. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | Kontrollerar om given kolumn är tom (innehåller inga data). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | Kontrollerar om en kolumn vid ett givet index är dold. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | Kontrollera om intervallet kunde tas bort. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | Kontrollerar om en rad vid ett givet index är dold. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | Länk till en xml-karta. |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | Slår samman ett specificerat cellområde till en enda cell. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | Slår samman ett specificerat cellområde till en enda cell. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | Slår samman ett specificerat cellområde till en enda cell. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | Flyttar området. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | Tar bort dubbletter av rader i arket. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | Tar bort dubbletter av värden i intervallet. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | Tar bort dubblettdata från intervallet. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | Tar bort alla formler och ersätter med värdet på formeln. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | Hämtar inställning för delsummor för intervallet. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | Ställer in bredden på den angivna kolumnen i normalvy. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | Ställer in kolumnbredden i enhet av tum i normalvy. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | Ställer in kolumnbredden i enhet pixlar i normal vy. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | Ställer in höjden på den angivna raden. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | Ställer in radhöjden i tumenhet. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | Ställer in radhöjden i pixelenhet. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | Ställer in bredden på kolumnen i en annan vy. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | Expanderar de grupperade raderna/kolumnerna. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Skapar delsummor för intervallet. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Skapar delsummor för intervallet. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | Delar upp texten i kolumnen till kolumner. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | Delar upp kolumner. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | Delar upp rader. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | Delar upp rader. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | Visar en kolumn |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | Visa flera kolumner. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | Visar en rad. |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | Visar de dolda raderna. |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | Tar bort ett specificerat intervall av sammanslagna celler. |

### Exempel

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Ställ in standard radhöjd
cells.StandardHeight = 20;
//Ställ in radhöjd
cells.SetRowHeight(2, 20.5);

//Ställ in standardkolumns bredd
cells.StandardWidth = 15;
//Ställ in kolumnbredd
cells.SetColumnWidth(3, 12.57);

//Sammanfoga celler
cells.Merge(5, 4, 2, 2);

//Sätt värden till celler
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Exportera data
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Ställ in standard radhöjd
cells.StandardHeight = 20
'Ställ in radhöjd
cells.SetRowHeight(2, 20.5)

'Ställ in standardkolumns bredd
cells.StandardWidth = 15
'Ställ in kolumnbredd
cells.SetColumnWidth(3, 12.57)

'Sammanfoga celler
cells.Merge(5, 4, 2, 2)

'Exportera data
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
