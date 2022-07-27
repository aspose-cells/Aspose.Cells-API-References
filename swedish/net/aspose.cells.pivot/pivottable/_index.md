---
title: PivotTable
second_title: Aspose.Cells för .NET API-referens
description: Sammanfattningsbeskrivning för pivottabell.
type: docs
weight: 4690
url: /sv/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Sammanfattningsbeskrivning för pivottabell.

```csharp
public class PivotTable : IDisposable
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Hämtar beskrivningen av alt text |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | Hämtar titeln på altertexten |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Hämtar automatisk formattyp för PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Returnerar ett PivotFields-objekt som inkluderar alla fält i pivottabellen report |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Returnerar ett PivotFields-objekt som för närvarande visas som kolumnfält. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Indikerar om pivottabellsrapporten visar totalsummor för kolumner. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | Hämtar kolumnrubriktexten för pivottabellen. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | Returnerar ett CellArea-objekt som representerar range som innehåller kolumnområdet i pivottabellsrapporten. Skrivskyddad. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | Anger om överväga inbyggd anpassad lista vid sortering av data |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Returnerar ett CellArea-objekt som representerar intervallet som innehåller dataområdet i listan mellan rubrikraden och infogningsraden. Skrivskyddad. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Hämtar ett PivotField-objekt som representerar alla datafält i en PivotTable. Skrivskyddat. Det skulle bara vara init när det finns två eller flera datafält i DataPiovtFiels. Det används bara för att lägga till DataPivotField till PivotTablen raden/kolumntabellen . område . Standard är i radområdet. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Hämtar ett PivotField-objekt som representerar alla datafält i en PivotTable. Skrivskyddat. Det skulle bara vara init när det finns två eller flera datafält i DataPiovtFiels. Det används bara för att lägga till DataPivotField till PivotTablen raden/kolumntabellen . område . Standard är i radområdet. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Hämtar och ställer in datakällan för pivottabellen. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | Indikerar om pivottabellsrapporten visar en anpassad sträng i celler som innehåller fel. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | Indikerar om objekt i rad- och kolumnområdena är synliga när dataområdet i pivottabellen är tomt. Standardvärdet är sant. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | Indikerar om pivottabellsrapporten visar en anpassad sträng i celler som innehåller nullvärden. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Anger ett booleskt värde som anger om användaren har tillåtelse att redigera cellerna i dataområdet för pivottabellen. Aktivera cellredigering i värdeområdet |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Hämtar om drilldown är aktiverat. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Indikerar om dialogrutan PivotTable Field är tillgänglig när användaren dubbelklickar på PivotTable-fältet. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | Hämtar om aktivera fältlistan för pivottabellen. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Indikerar om PivotTable Wizard är tillgänglig. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | Hämtar strängen som visas i celler som innehåller errors när egenskapen DisplayErrorString är true. Standardvärdet är en tom sträng. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Hämtar den externa anslutningsdatakällan. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | Anger ett booleskt värde som anger om fält i pivottabellen sorteras i icke-standardordning i fältlistan. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Returnerar textsträngsetiketten som visas i kolumnen eller radrubriken. Standardvärdet är strängen "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Indikerar om tomma rader ska läggas till. Den här egenskapen gäller endast för de automatiska formattyperna för pivottabell som behöver lägga till tomma rader. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Anger indragningsstegringen för kompakt axel och kan användas för att ställa in rapportlayouten till Compact Form. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Indikerar om pivottabellsrapporten formateras automatiskt. Kryssrutan "autoformat tabell " som är i pivoteringsalternativ för Excel 2003 Kryssrutan "autofit kolumnbredd vid uppdatering" som är i pivottabell Alternativ :Layoutformat för Excel 2000d_x00 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Anger om pivottabellen är kompatibel för Excel2003 vid uppdatering av pivottabell, om sant, en sträng måste vara mindre än eller lika med 255 tecken, så om strängen är större än 255 tecken, kommer den att trunkeras. om false, kommer en sträng inte att ha den ovan nämnda begränsningen. Standardvärdet är true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | Indikerar om pivottabellsrapporten visar klassisk pivotbar layout. (möjliggör att dra fält i rutnätet) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Anger ett booleskt värde som anger om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | Indikerar om pivottabellen är vald. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | En bit som anger om rubriker för pivotobjekt på radaxeln upprepas på varje utskriven sida för pivotfält i tabellform. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Indikerar om pivottabellsrapporten endast beräknas om på användarens begäran. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Indikerar om den angivna pivottabellrapportens ytterradpost, kolumnpost, delsumma, och totalsumma etiketter använder sammanslagna celler. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Anger ett booleskt värde som anger om fälten i en pivottabell kan ha flera filter inställda på dem. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | Hämtar namnet på pivottabellen |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | Hämtar strängen som visas i celler som innehåller null values när egenskapen DisplayNullString är true. Standardvärdet är en tom sträng. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Hämtar i vilken ordning sidfälten läggs till i pivottabellsrapportens layout. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Returnerar ett PivotFields-objekt som för närvarande visas som sidfält. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | Hämtar antalet sidfält i varje kolumn eller rad i pivottabellsrapporten. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Returnerar ett PivotFilterCollection-objekt. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Hämtar formatvillkoren för pivottabellen. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Hämtar och ställer in det vridbara stilnamnet. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Hämtar och ställer in den inbyggda pivottabellstilen. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Indikerar om formateringen bevaras när pivottabellen uppdateras eller räknas om. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Anger ett booleskt värde som anger om borrindikatorer ska skrivas ut. skriv ut expandera/komprimera knappar när de visas på vridbar. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Indikerar om utskriftsrubriken för kalkylbladet är inställda baserat i pivottabellsrapporten. Standardvärdet är false. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Indikerar om Uppdatera data eller inte. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Indikerar om Uppdatera data vid öppning av fil. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | Hämtar datumet när pivottabellen senast uppdaterades. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Hämtar namnet på användaren som senast uppdaterade pivottabellen |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Returnerar ett PivotFields-objekt som för närvarande visas som radfält. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Indikerar om pivottabellsrapporten visar totalsummor för rader. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | Hämtar radrubriktexten för pivottabellen. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | Returnerar ett CellArea-objekt som representerar range som innehåller radområdet i pivottabellsrapporten. Skrivskyddad. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | Anger om data för pivottabellsrapporten sparas med arbetsboken. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | Anger ett booleskt värde som anger om verktygstips ska visas för pivottabelldataceller. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Hämtar om expandera/komprimera knappar visas. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Anger ett booleskt värde som anger om tomma kolumner ska inkluderas i tabellen |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Anger ett booleskt värde som anger om tomma rader ska inkluderas i tabellen. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Anger ett booleskt värde som indikerar om medlemsegenskapsinformation ska utelämnas från pivottabellens verktygstips. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Indikerar om kolumnrubriken i pivottabellen ska ha stilen tillämpad. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Indikerar om formatering av kolumnrand används. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Indikerar om formatering av kolumnrand används. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Indikerar om radhuvudet i pivottabellen ska ha stilen tillämpad. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Indikerar om radrandsformatering tillämpas. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Indikerar om radrubrik visas i pivottabellen report Indikerar om Visa fälttexter och filter drop downs |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Anger ett booleskt värde som anger om visa värden row. visa värdena row |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Indikerar om dolda sidfältsobjekt i pivottabellsrapporten ingår i rad- och kolumndelsummor, blocksummor och totalsummor. Standardvärdet är False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | Returnerar ett CellArea-objekt som representerar intervallet som innehåller hela pivottabellsrapporten, men som inte inkluderar sidfält. Skrivskyddad. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | Returnerar ett CellArea-objekt som representerar intervallet som innehåller hela pivottabellsrapporten, innehåller sidfält. Skrivskyddad. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | Får en sträng sparad med pivottabellsrapporten. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Lägger till ett beräknat fält till pivotfältet och dra det till dataområdet. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Lägger till ett beräknat fält till pivotfält. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Lägger till fältet till det specifika området. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Lägger till fältet till det specifika området. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Lägger till fältet till det specifika området. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Beräknar pivotables data till celler. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Beräknar pivotables räckvidd. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Ställ in pivotablens källdata. Blad1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | Rensa pivottabellens data och formatering |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Kopierar namngiven stil från en annan pivottabell. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Hämtar specifika fält efter fälttyp. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Formatera cellen i det vridbara området |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Formatera hela cellen i det vridbara området |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Formatera raddata i det vridbara området |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Hämtar cellobjektet med visningsnamnet för PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Hämtar pivottabellerna för barn som använder denna pivottabellsdata som datakälla. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | hämta pivottabellens radindexlista över horisontella sidbrytningar |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Hämta pivottables källdata. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Uppdaterar pivotablens data och inställning från dess datakälla. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Tar bort ett fält från specifikt fältområde |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Ta bort fält från specifikt fält area |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Tar bort ett fält från specifikt fältområde |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Ställer in automatisk fältgrupp efter pivottabellen. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Ställer in automatisk fältgrupp efter pivottabellen. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | Ställer in manuell fältgrupp efter pivottabellen. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | Ställer in manuell fältgrupp efter pivottabellen. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | Ställer in manuell fältgrupp efter pivottabellen. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Ställer in manuell fältgrupp efter pivottabellen. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Anger att dela upp gruppering efter pivottabellen |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Anger att dela upp gruppering efter pivottabellen |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | Layouter pivottabellen i kompakt form. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | Layouter pivottabellen i konturform. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | Layouter pivottabellen i tabellform. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Visa alla rapportfiltersidor enligt PivotField, PivotField måste finnas i PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | Visa alla rapportfiltersidor enligt positionsindex i PageFields |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Visa alla rapportfiltersidor enligt PivotFields namn, PivotField måste finnas i PageFields. |

### Exempel

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Ändra PivotFields attribut
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Lägg till PivotFilter
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

//Lägg till PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

//gör dina affärer

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Lägg till PivotFilter
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Lägg till PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Se även

* namnutrymme [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
