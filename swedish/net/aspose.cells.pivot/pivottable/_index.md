---
title: "Klass PivotTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTable-klass. Sammanfattande beskrivning för PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Sammanfattande beskrivning för PivotTable.

```csharp
public class PivotTable : IDisposable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | Hämtar beskrivningen av alternativ text. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | Hämtar och anger titeln för den alternativa texten. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | Anger om kolumnbredden ska anpassas automatiskt vid uppdatering |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | Hämtar och anger automatisk formattyp för PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | Returnerar alla grundläggande pivotfält i PivotTable. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | Returnerar ett PivotFields-objekt som för närvarande visas som kolumnfält. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Obsolete.**) Anger om PivotTable‑rapporten visar totalsummor för kolumner. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | Hämtar och anger den anpassade rubriken för kolumnrubriken i pivottabellen. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | Returnerar ett CellArea‑objekt som representerar det område som innehåller kolumnområdet i pivottabellsrapporten. Endast läsning. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | Hämtar de villkorsformat som används i pivottabellen. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | Anger om inbyggda anpassade listor ska beaktas vid sortering av data. |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | Returnerar ett [`CellArea`](../../aspose.cells/cellarea/)‑objekt som representerar det område som innehåller dataområdet i listan mellan rubrikraden och infogningsraden. Endast läsning. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Obsolete.**) Hämtar ett [`PivotField`](../pivotfield/)‑objekt som representerar alla datafält i en pivottabell. Endast läsning. Det skapas endast när det finns två eller fler datafält i datatområdet. Som standard är det i radområdet. Du kan dra det till rad‑/kolumnområdet med metoden PivotTable.AddFieldToArea(). |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | Hämtar och anger namnet på fältrubriken för värdeområdet i pivottabellen. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | Hämtar en [`PivotFieldCollection`](../pivotfieldcollection/) som representerar alla datafält i en pivottabell. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | Hämtar och anger datakällan för pivottabellen. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | Anger om pivottabellsrapporten visar en anpassad sträng i celler som innehåller fel. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | Anger om objekt i rad‑ och kolumnområdena är synliga när dataområdet i pivottabellen är tomt. Standardvärdet är sant. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | Anger om pivottabellsrapporten visar en anpassad sträng om värdet är null. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | Anger ett booleskt värde som visar om användaren får redigera cellerna i dataområdet i pivottabellen. Standardvärdet är falskt. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | Anger om drill‑down är aktiverat. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | Anger om dialogrutan för pivottabellfält är tillgänglig när användaren dubbelklickar på pivottabellfältet. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | Anger om fältlistan för pivottabellen är tillgänglig i Excels vy. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | Anger om pivottabellguiden är tillgänglig. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | Hämtar den sträng som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolete.**) Hämtar den externa anslutningsdatakällan. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | Anger om fält i pivottabellen sorteras i en icke‑standardordning i fältlistan. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | Hämtar området för filterregionen. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | Returnerar etiketten som visas i rubriken för total‑kolumnen eller -raden. Standardvärdet är strängen "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolete.**) Anger om tomma rader ska läggas till. Denna egenskap gäller endast för pivottabellens autoformat‑typer som kräver tomma rader. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | Anger indenteringsökningen för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | Anger om pivottabellsrapporten formateras automatiskt. Kryssrutan "autoformat table" som finns i pivottabellalternativet för Excel 2003. |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | Anger om PivotTable är kompatibel med Excel2003 vid uppdatering av PivotTable; om true måste en sträng vara mindre än eller lika med 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. Om false har en sträng inte den nämnda begränsningen. Standardvärdet är true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | Anger om PivotTable‑rapporten visar klassisk pivottable‑layout. (möjliggör att dra fält i rutnätet) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolete.**) Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | Anger om denna PivotTable är markerad. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolete.**) Anger om PivotItem‑namn ska upprepas högst upp på varje utskriven sida. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | Anger om PivotTable‑rapporten beräknas om endast på begäran av användaren. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | Hämtar eller anger om rad-/kolumnfältetiketter som sträcker sig över flera celler ska slås ihop. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolete.**) Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | Hämtar namnet på PivotTable |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är true. Standardvärdet är en tom sträng. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | Hämtar och anger ordningen i vilken sidfält läggs till i PivotTable‑rapportens layout. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | Returnerar en [`PivotFieldCollection`](../pivotfieldcollection/) som för närvarande visas som sidfält. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | Hämtar datakällan. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | Returnerar alla filter i pivottabellen. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolete.**) Hämtar formatvillkoren för pivottabellen. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | Hämtar alla cellformat som tillämpas på denna pivottabell. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | Hämtar TableStyle‑inställningarna för denna pivottabell. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | Hämtar eller anger stilnamnet för pivottabellen. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | Hämtar och anger den inbyggda pivottabellstilen. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | Anger om cellformatering ([`PivotTableFormat`](../pivottableformat/)) ska bevaras när pivottabellen uppdateras eller beräknas om. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolete.**) Anger om cellformatering ([`PivotTableFormat`](../pivottableformat/)) bevaras när PivotTable uppdateras eller beräknas om. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. Skriv ut expandera/komprimera‑knappar när de visas i pivottabellen. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | Anger om utskriftsrubrikerna för kalkylbladet sätts baserat på PivotTable‑rapporten. Standardvärdet är false. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | Anger om data ska uppdateras vid öppning av filen. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | Hämtar det senaste datumet och tiden då PivotTable uppdaterades. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | Hämtar namnet på den senaste användaren som uppdaterade denna PivotTable |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | Anger om rubriker för pivotelement i radområdet upprepas på varje utskriven sida för pivofält i tabellformat. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | Returnerar en [`PivotFieldCollection`](../pivotfieldcollection/) som för närvarande visas som radfält. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Obsolete.**) Anger om totalsummor för rader i denna pivottabell ska visas. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | Hämtar och anger anpassad rubrik för radhuvudet i denna PivotTable. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | Returnerar ett CellArea-objekt som representerar det område som innehåller radområdet i PivotTable‑rapporten. Endast läsning. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | Anger om data för PivotTable‑rapporten sparas med arbetsboken. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | Anger om totalsummor för kolumner i denna pivottabell ska visas. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | Anger om verktygstips ska visas för PivotTable‑dataceller. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | Hämtar och anger om expandera/komprimera‑knappar ska visas. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | Anger om tomma kolumner ska inkluderas i tabellen |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | Anger om tomma rader ska inkluderas i tabellen. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | Om rubriker för datafält och pivofält ska visas på radaxeln och kolumnaxeln i PivotTable‑vyn. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | Specificerar ett booleskt värde som anger om medlems‑egenskapsinformation ska utelämnas från PivotTable‑verktygstips. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | Anger om kolumnrubriken i pivottabellen ska ha stilen tillämpad. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | Anger om stripe‑formatering tillämpas för kolumnen. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | Anger om kolumnformatering har tillämpats. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | Anger om radhuvudet i pivottabellen ska ha stilen tillämpad. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | Anger om radstripe‑formatering tillämpas. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | Anger om totalsummor för rader i pivottabellen ska visas. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Obsolete.**) Anger om radhuvudrubrik visas i PivotTable‑rapporten Anger om fält‑rubriker och filter‑rullgardiner ska visas |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | Anger om värderadsrad visas. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | Hämtar datakälltyp för pivottabellen. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | Anger om dolda sidfältsposter i PivotTable‑rapporten inkluderas i rad‑ och kolumnsubtotals, block‑totals och totalsummor. Standardvärdet är False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | Returnerar ett CellArea‑objekt som representerar det område som innehåller hela PivotTable‑rapporten, men som inte inkluderar sidfält. Endast läsning. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | Returnerar ett CellArea-objekt som representerar intervallet som innehåller hela PivotTable-rapporten, inklusive sidfält. Endast läsning. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | Hämtar och anger en användardefinierad sträng som är associerad med den här PivotTable-vyn. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | Representerar det tomma området längst upp till höger i PivotTable (längst upp till vänster för RTL-ark). |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | Hämtar ett [`PivotField`](../pivotfield/)‑objekt som representerar alla datafält i en PivotTable. Endast läsning. Det skapas endast när det finns två eller fler datafält i datatregionen. Som standard är det i radregionen. Du kan dra det till rad‑/kolumnregionen med metoden PivotTable.AddFieldToArea(). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | Lägger till ett beräknat fält till pivotfältet och drar det till dataområdet. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | Lägger till ett beräknat fält till pivotfältet. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | Lägger till fältet i det specifika området. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | Lägger till fältet i det specifika området. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | Lägger till fältet i det specifika området. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | Beräknar pivottabellens data till celler. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | Beräknar pivottabell med alternativ. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | Beräknar pivottabellens område. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | Ändra datakälla för pivottabellen. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | Ta bort alla fält från regioner. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | Rensa data och formatering för PivotTable-vyn. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | Rensar alla filter i denna pivottabell. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | Kopierar namngiven stil från en annan pivottabell. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | Exporterar pivottabellsvyn som JSON. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Obsolete.**) Hämtar de specifika fälten efter fälttypen. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | Formaterar markerat område i PivotTable. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | Formaterar markerat område i PivotTable. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | Formaterar cellen i pivottabellområdet |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | Formatera alla celler i pivottabellområdet |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | Formatera raddata i pivottabellområdet |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | Hämtar området som innehåller fältknappen. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | Hämtar [`Cell`](../../aspose.cells/cell/)‑objektet via visningsnamnet för PivotField. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Obsolete.**) Hämtar de underliggande PivotTable‑tabellerna som använder denna PivotTables data som datakälla. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | Hämtar alla `PivotTable`s som använder denna PivotTable som deras datakälla. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | Hämtar den specifika listan med pivotfält efter regionen. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Obsolete.**) Hämtar pivottabellens radindexlista för horisontella sidbrytningar |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | Hämtar horisontella sidbrytningar för denna pivottabell. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | Hämtar namnen på externa datakällans anslutningar. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | Hämtar alla pivottabeller med samma pivot cache. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | Hämta datakällan för denna pivottabell. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | Hämta datakällan för denna pivottabell. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | Hämtar de externa anslutningsdatakällorna. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | Flytta ett objekt upp eller ner. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | Uppdatera [`PivotCache`](./pivotcache/) från datakälla och beräkna data och stil för pivotvy. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | Uppdatera [`PivotCache`](./pivotcache/) från datakälla och beräkna data och stil för pivotvy. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) Uppdaterar data från dess datakälla till pivotcache. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) Uppdaterar pivottabellens data och inställningar från dess datakälla med alternativ. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | Tar bort ett fält från ett specifikt pivotområde. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | Ta bort fält från specifikt fältområde |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | Tar bort ett fält från specifikt fältområde |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | Välj ett område i pivottabellvyn. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | Visa detaljerna för ett objekt i dataområdet i en ny tabell. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | Formaterar pivottabellvyn i kompakt form. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | Formaterar pivottabellen i konturform. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | Formaterar pivottabellen i tabellform. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | Visa alla rapportfilter‑sidor enligt PivotField, PivotField måste vara placerad i PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | Visa alla rapportfilter‑sidor enligt positionsindexet i PageFields. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | Visa alla rapportfilter‑sidor enligt PivotField:s namn, PivotField måste vara placerad i PageFields. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ange exempeldata
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Skapa pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // Lägg till fält
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Formatera pivottabellen
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Anpassa radfältet
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // Uppdatera och beräkna data
            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsboken
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


