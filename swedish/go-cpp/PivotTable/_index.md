---
title: "PivotTable-klass"
linktitle: "PivotTable"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotTable-klass. Inkapslar objektet som representerar pivottabell i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivottable/
---

## PivotTable class

Sammanfattande beskrivning för PivotTable.

```go

type PivotTable struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [Dispose](./dispose/) | Utför applikationsdefinierade uppgifter som är kopplade till frigöring, släppande eller återställning av ohanterade resurser. |
| [GetPivotCache](./getpivotcache/) | Hämtar datakällan. |
| [IsExcel2003Compatible](./isexcel2003compatible/) | Anger om PivotTable är kompatibel med Excel2003 vid uppdatering av PivotTable, om true måste en sträng vara kortare än eller lika med 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. om false kommer en sträng inte att ha den ovan nämnda begränsningen. Standardvärdet är true. |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | Anger om PivotTable är kompatibel med Excel2003 vid uppdatering av PivotTable, om true måste en sträng vara kortare än eller lika med 255 tecken, så om strängen är längre än 255 tecken kommer den att trunkeras. om false kommer en sträng inte att ha den ovan nämnda begränsningen. Standardvärdet är true. |
| [GetRefreshedByWho](./getrefreshedbywho/) | Hämtar namnet på den senaste användaren som uppdaterade denna PivotTable |
| [GetRefreshDate](./getrefreshdate/) | Hämtar det senaste datumet och tiden då PivotTable uppdaterades. |
| [GetPivotTableStyle](./getpivottablestyle/) | Hämtar TableStyle-inställningarna för denna pivottabell. |
| [SetPivotTableStyle](./setpivottablestyle/) | Hämtar TableStyle-inställningarna för denna pivottabell. |
| [GetPivotTableStyleName](./getpivottablestylename/) | Hämtar eller anger stilnamnet för pivottabellen. |
| [SetPivotTableStyleName](./setpivottablestylename/) | Hämtar eller anger stilnamnet för pivottabellen. |
| [GetPivotTableStyleType](./getpivottablestyletype/) | Hämtar och anger den inbyggda pivottabellstilen. |
| [SetPivotTableStyleType](./setpivottablestyletype/) | Hämtar och anger den inbyggda pivottabellstilen. |
| [CopyStyle](./copystyle/) | Kopierar namngiven stil från en annan pivottabell. |
| [ShowReportFilterPage](./showreportfilterpage/) | Visa alla rapportfilter‑sidor enligt PivotField, PivotField måste vara placerad i PageFields. |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | Visa alla rapportfilter‑sidor enligt PivotFields namn, PivotField måste vara placerad i PageFields. |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | Visa alla rapportfilter‑sidor enligt positionsindexet i PageFields |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | Tar bort ett fält från ett specifikt fältområde |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | Tar bort ett fält från ett specifikt pivottområde. |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | Ta bort fält från specifikt fältområde |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | Lägger till fältet i det specifika området. |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | Lägger till fältet i det specifika området. |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | Lägger till fältet i det specifika området. |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | Lägger till ett beräknat fält till pivottfältet. |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | Lägger till ett beräknat fält till pivottfältet och drar det till dataområdet. |
| [GetFields](./getfields/) | Hämtar den specifika listan med pivottfält efter regionen. |
| [GetColumnFields](./getcolumnfields/) | Returnerar ett PivotFields-objekt som för närvarande visas som kolumnfält. |
| [GetRowFields](./getrowfields/) | Returnerar ett PivotFields-objekt som för närvarande visas som radfält. |
| [GetPageFields](./getpagefields/) | Returnerar ett PivotFields-objekt som för närvarande visas som sidfält. |
| [GetDataFields](./getdatafields/) | Hämtar ett PivotField-objekt som representerar alla datafält i en PivotTable. Läs‑endast. Det initieras endast när det finns två eller fler datafält i DataPiovtFiels. Det används endast för att lägga till DataPivotField till PivotTables rad‑/kolumnområde. Standard är i radområdet. |
| [GetValuesField](./getvaluesfield/) | Hämtar ett PivotField-objekt som representerar alla datafält i en PivotTable. Läs‑endast. Det skapas endast när det finns två eller fler datafält i Data‑regionen. Som standard är det i radregionen. Du kan dra det till rad‑/kolumnregionen med metoden PivotTable.AddFieldToArea(). |
| [GetBaseFields](./getbasefields/) | Returnerar alla grundläggande pivottfält i PivotTable. |
| [GetPivotFilters](./getpivotfilters/) | Returnerar alla filter för pivotfält i pivottabellen. |
| [GetButtonArea](./getbuttonarea/) | Hämtar området som innehåller fältknappen. |
| [GetTopRightArea](./gettoprightarea/) | Representerar det tomma området högst upp till höger i pivottabellen (uppe till vänster för RTL-ark). |
| [GetFilterArea](./getfilterarea/) | Hämtar området för filterregionen. |
| [GetColumnRange](./getcolumnrange/) | Returnerar ett CellArea-objekt som representerar det område som innehåller kolumnområdet i pivottabellrapporten. Endast läsning. |
| [GetRowRange](./getrowrange/) | Returnerar ett CellArea-objekt som representerar det område som innehåller radområdet i pivottabellrapporten. Endast läsning. |
| [GetDataBodyRange](./getdatabodyrange/) | Returnerar ett CellArea-objekt som representerar det område som innehåller dataområdet i listan mellan rubrikraden och infogningsraden. Endast läsning. |
| [GetTableRange1](./gettablerange1/) | Returnerar ett CellArea-objekt som representerar det område som innehåller hela pivottabellrapporten, men exkluderar sidfält. Endast läsning. |
| [GetTableRange2](./gettablerange2/) | Returnerar ett CellArea-objekt som representerar det område som innehåller hela pivottabellrapporten, inklusive sidfält. Endast läsning. |
| [MoveTo_Int_Int](./moveto_int_int/) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [MoveTo_String](./moveto_string/) | Flyttar pivottabellen till en annan plats i kalkylbladet. |
| [IsGridDropZones](./isgriddropzones/) | Anger om pivottabellrapporten visar klassisk pivottabelllayout (möjliggör dragning av fält i rutnätet). |
| [SetIsGridDropZones](./setisgriddropzones/) | Anger om pivottabellrapporten visar klassisk pivottabelllayout (möjliggör dragning av fält i rutnätet). |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | Anger om totalsummor ska visas för kolumnerna i denna pivottabell. |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | Anger om totalsummor ska visas för kolumnerna i denna pivottabell. |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | Anger om totalsummor ska visas för raderna i pivottabellen. |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | Anger om totalsummor ska visas för raderna i pivottabellen. |
| [GetDisplayNullString](./getdisplaynullstring/) | Anger om pivottabellrapporten visar en anpassad sträng när värdet är null. |
| [SetDisplayNullString](./setdisplaynullstring/) | Anger om pivottabellrapporten visar en anpassad sträng när värdet är null. |
| [GetNullString](./getnullstring/) | Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är sann. Standardvärdet är en tom sträng. |
| [SetNullString](./setnullstring/) | Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är sann. Standardvärdet är en tom sträng. |
| [GetDisplayErrorString](./getdisplayerrorstring/) | Anger om pivottabellrapporten visar en anpassad sträng i celler som innehåller fel. |
| [SetDisplayErrorString](./setdisplayerrorstring/) | Anger om pivottabellrapporten visar en anpassad sträng i celler som innehåller fel. |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | Hämtar och anger namnet på rubriken för värdeområdesfältet i pivottabellen. |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | Hämtar och anger namnet på rubriken för värdeområdesfältet i pivottabellen. |
| [GetErrorString](./geterrorstring/) | Hämtar strängen som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng. |
| [SetErrorString](./seterrorstring/) | Hämtar strängen som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng. |
| [IsAutoFormat](./isautoformat/) | Anger om pivottabellrapporten är automatiskt formaterad. Kryssrutan "autoformat table" finns i pivottabellsalternativet för Excel 2003. |
| [SetIsAutoFormat](./setisautoformat/) | Anger om pivottabellrapporten är automatiskt formaterad. Kryssrutan "autoformat table" finns i pivottabellsalternativet för Excel 2003. |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | Anger om kolumnbredden ska anpassas automatiskt vid uppdatering. |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | Anger om kolumnbredden ska anpassas automatiskt vid uppdatering. |
| [GetAutoFormatType](./getautoformattype/) | Hämtar och anger den automatiska formattypen för pivottabellen. |
| [SetAutoFormatType](./setautoformattype/) | Hämtar och anger den automatiska formattypen för pivottabellen. |
| [GetMergeLabels](./getmergelabels/) | Anger om rad- eller kolumnrubriker som sträcker sig över flera celler ska slås ihop till en enda cell. |
| [SetMergeLabels](./setmergelabels/) | Anger om rad- eller kolumnrubriker som sträcker sig över flera celler ska slås ihop till en enda cell. |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | Anger om cellformatering (PivotTableFormat) ska bevaras när pivottabellen uppdateras eller beräknas om. |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | Anger om cellformatering (PivotTableFormat) ska bevaras när pivottabellen uppdateras eller beräknas om. |
| [GetShowDrill](./getshowdrill/) | Hämtar och anger om expandera/komprimera‑knappar ska visas. |
| [SetShowDrill](./setshowdrill/) | Hämtar och anger om expandera/komprimera‑knappar ska visas. |
| [GetEnableDrilldown](./getenabledrilldown/) | Anger om drilldown är aktiverat. |
| [SetEnableDrilldown](./setenabledrilldown/) | Anger om drilldown är aktiverat. |
| [GetEnableFieldDialog](./getenablefielddialog/) | Anger om dialogrutan för PivotTable-fält är tillgänglig när användaren dubbelklickar på PivotTable-fältet. |
| [SetEnableFieldDialog](./setenablefielddialog/) | Anger om dialogrutan för PivotTable-fält är tillgänglig när användaren dubbelklickar på PivotTable-fältet. |
| [GetEnableFieldList](./getenablefieldlist/) | Anger om fältlistan för PivotTable är tillgänglig i Excel-vyn. |
| [SetEnableFieldList](./setenablefieldlist/) | Anger om fältlistan för PivotTable är tillgänglig i Excel-vyn. |
| [GetEnableWizard](./getenablewizard/) | Anger om PivotTable-guiden är tillgänglig. |
| [SetEnableWizard](./setenablewizard/) | Anger om PivotTable-guiden är tillgänglig. |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | Anger om dolda sidfältsposter i PivotTable-rapporten inkluderas i rad- och kolumnsubtotaler, blocktotaler och totalsummor. Standardvärdet är False. |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | Anger om dolda sidfältsposter i PivotTable-rapporten inkluderas i rad- och kolumnsubtotaler, blocktotaler och totalsummor. Standardvärdet är False. |
| [GetGrandTotalName](./getgrandtotalname/) | Returnerar etiketten som visas i rubriken för grand total‑kolumnen eller -raden. Standardvärdet är strängen "Grand Total". |
| [SetGrandTotalName](./setgrandtotalname/) | Returnerar etiketten som visas i rubriken för grand total‑kolumnen eller -raden. Standardvärdet är strängen "Grand Total". |
| [GetManualUpdate](./getmanualupdate/) | Anger om PivotTable-rapporten endast beräknas om användaren begär det. |
| [SetManualUpdate](./setmanualupdate/) | Anger om PivotTable-rapporten endast beräknas om användaren begär det. |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem. |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem. |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | Anger ett booleskt värde som visar om användaren får redigera cellerna i datatområdet för pivottabellen. Aktivera cellredigering i värdeområdet. |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | Anger ett booleskt värde som visar om användaren får redigera cellerna i datatområdet för pivottabellen. Aktivera cellredigering i värdeområdet. |
| [GetShowDataTips](./getshowdatatips/) | Anger om verktygstips ska visas för PivotTable-dataceller. |
| [SetShowDataTips](./setshowdatatips/) | Anger om verktygstips ska visas för PivotTable-dataceller. |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | Anger ett booleskt värde som visar om medlemsegenskapsinformation ska utelämnas från PivotTable-verktygstips. |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | Anger ett booleskt värde som visar om medlemsegenskapsinformation ska utelämnas från PivotTable-verktygstips. |
| [GetShowValuesRow](./getshowvaluesrow/) | Anger om värderadsraden visas. |
| [SetShowValuesRow](./setshowvaluesrow/) | Anger om värderadsraden visas. |
| [GetShowEmptyCol](./getshowemptycol/) | Anger om tomma kolumner ska inkluderas i tabellen. |
| [SetShowEmptyCol](./setshowemptycol/) | Anger om tomma kolumner ska inkluderas i tabellen. |
| [GetShowEmptyRow](./getshowemptyrow/) | Anger om tomma rader ska inkluderas i tabellen. |
| [SetShowEmptyRow](./setshowemptyrow/) | Anger om tomma rader ska inkluderas i tabellen. |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | Anger om fält i PivotTable är sorterade i en icke‑standardordning i fältlistan. |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | Anger om fält i PivotTable är sorterade i en icke‑standardordning i fältlistan. |
| [GetPrintDrill](./getprintdrill/) | Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. Skriv ut expandera/komprimera‑knappar när de visas i pivottabellen. |
| [SetPrintDrill](./setprintdrill/) | Anger ett booleskt värde som visar om drill‑indikatorer ska skrivas ut. Skriv ut expandera/komprimera‑knappar när de visas i pivottabellen. |
| [GetAltTextTitle](./getalttexttitle/) | Hämtar och anger titeln för alternativ text. |
| [SetAltTextTitle](./setalttexttitle/) | Hämtar och anger titeln för alternativ text. |
| [GetAltTextDescription](./getalttextdescription/) | Hämtar beskrivningen av alternativ text. |
| [SetAltTextDescription](./setalttextdescription/) | Hämtar beskrivningen av alternativ text. |
| [GetName](./getname/) | Hämtar namnet på PivotTable. |
| [SetName](./setname/) | Hämtar namnet på PivotTable. |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | Hämtar och anger den anpassade rubriken för kolumnrubriken i PivotTable. |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | Hämtar och anger den anpassade rubriken för kolumnrubriken i PivotTable. |
| [GetIndent](./getindent/) | Anger indenteringssteget för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form. |
| [SetIndent](./setindent/) | Anger indenteringssteget för kompakt axel och kan användas för att ställa in rapportlayouten till kompakt form. |
| [GetRowHeaderCaption](./getrowheadercaption/) | Hämtar och anger anpassad rubrik för radrubriken i denna PivotTable. |
| [SetRowHeaderCaption](./setrowheadercaption/) | Hämtar och anger anpassad rubrik för radrubriken i denna PivotTable. |
| [GetShowHeaders](./getshowheaders/) | Om datafältetiketter och pivotfältetiketter ska visas på radaxeln och kolumnaxeln i PivotTable-vyn. |
| [SetShowHeaders](./setshowheaders/) | Om datafältetiketter och pivotfältetiketter ska visas på radaxeln och kolumnaxeln i PivotTable-vyn. |
| [GetCustomListSort](./getcustomlistsort/) | Anger om inbyggda anpassade listor ska beaktas vid sortering av data. |
| [SetCustomListSort](./setcustomlistsort/) | Anger om inbyggda anpassade listor ska beaktas vid sortering av data. |
| [GetConditionalFormats](./getconditionalformats/) | Hämtar de villkorliga formaten för pivottabellen. |
| [GetPageFieldOrder](./getpagefieldorder/) | Hämtar och anger den ordning i vilken sidfält läggs till i PivotTable-rapportens layout. |
| [SetPageFieldOrder](./setpagefieldorder/) | Hämtar och anger den ordning i vilken sidfält läggs till i PivotTable-rapportens layout. |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten. |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten. |
| [GetTag](./gettag/) | Hämtar och anger en användardefinierad sträng som är associerad med den här PivotTable‑vyn. |
| [SetTag](./settag/) | Hämtar och anger en användardefinierad sträng som är associerad med den här PivotTable‑vyn. |
| [GetSaveData](./getsavedata/) | Anger om data för PivotTable‑rapporten sparas med arbetsboken. |
| [SetSaveData](./setsavedata/) | Anger om data för PivotTable‑rapporten sparas med arbetsboken. |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | Anger om data ska uppdateras vid öppning av filen. |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | Anger om data ska uppdateras vid öppning av filen. |
| [GetSourceType](./getsourcetype/) | Hämtar datakällans typ för pivottabellen. |
| [GetSourceDataConnections](./getsourcedataconnections/) | Hämtar de externa anslutningsdatakällorna. |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | Hämtar namnen på externa datakällans anslutningar. |
| [GetDataSource](./getdatasource/) | Hämtar och anger datakällan för pivottabellen. |
| [SetDataSource](./setdatasource/) | Hämtar och anger datakällan för pivottabellen. |
| [ChangeDataSource](./changedatasource/) | Ändra datakällan för pivottabellen. |
| [GetSource](./getsource/) | Hämta datakällan för denna pivottabell. |
| [GetSource_Bool](./getsource_bool/) | Hämta datakällan för denna pivottabell. |
| [Refresh](./refresh/) | Uppdatera PivotCache från datakällan och beräkna data och stil för pivotovyn. |
| [CalculateData](./calculatedata/) | Beräknar pivottabellens data till celler. |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | Beräknar pivottabell med alternativ. |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | Hämtar alla pivottabeller med samma pivotcache. |
| [ClearData](./cleardata/) | Rensa data och formatering för PivotTable‑vyn. |
| [ClearFilters](./clearfilters/) | Rensar alla filter för denna pivottabell. |
| [ClearAll](./clearall/) | Ta bort alla fält från regioner. |
| [CalculateRange](./calculaterange/) | Beräknar pivottabellens område. |
| [FormatAll](./formatall/) | Formatera alla celler i pivottabellområdet |
| [FormatRow](./formatrow/) | Formatera raddata i pivottabellområdet |
| [Format_PivotArea_Style](./format_pivotarea_style/) | Formaterar markerat område i PivotTable. |
| [Format_CellArea_Style](./format_cellarea_style/) | Formaterar markerat område i PivotTable. |
| [Format_Int_Int_Style](./format_int_int_style/) | Formaterar cellen i pivottabellområdet |
| [SelectArea](./selectarea/) | Markera ett område i pivottabellvyn. |
| [ShowDetail](./showdetail/) | Visa detaljerna för ett objekt i dataregionen i en ny tabell. |
| [GetPivotFormats](./getpivotformats/) | Hämtar alla format som tillämpas på PivotTable. |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | Anger om rubriker för pivotelement på radområdet upprepas på varje utskriven sida för pivottfält i tabellform. |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | Anger om rubriker för pivotelement på radområdet upprepas på varje utskriven sida för pivottfält i tabellform. |
| [GetPrintTitles](./getprinttitles/) | Anger om utskriftstitlarna för kalkylbladet är inställda baserat på PivotTable-rapporten. Standardvärdet är falskt. |
| [SetPrintTitles](./setprinttitles/) | Anger om utskriftstitlarna för kalkylbladet är inställda baserat på PivotTable-rapporten. Standardvärdet är falskt. |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | Anger om objekt i rad- och kolumnområdena är synliga när datat området i PivotTable är tomt. Standardvärdet är sant. |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | Anger om objekt i rad- och kolumnområdena är synliga när datat området i PivotTable är tomt. Standardvärdet är sant. |
| [IsSelected](./isselected/) | Anger om denna PivotTable är markerad. |
| [SetIsSelected](./setisselected/) | Anger om denna PivotTable är markerad. |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | Anger om radrubriken i pivottabellen ska ha stilen tillämpad. |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | Anger om radrubriken i pivottabellen ska ha stilen tillämpad. |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | Anger om kolumnrubriken i pivottabellen ska ha stilen tillämpad. |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | Anger om kolumnrubriken i pivottabellen ska ha stilen tillämpad. |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | Anger om radrandig formatering tillämpas. |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | Anger om radrandig formatering tillämpas. |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | Anger om randig formatering tillämpas för kolumn. |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | Anger om randig formatering tillämpas för kolumn. |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | Anger om kolumnformateringen är tillämpad. |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | Anger om kolumnformateringen är tillämpad. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Hämtar horisontella sidbrytningar för denna pivottabell. |
| [ShowInCompactForm](./showincompactform/) | Layoutar PivotTable-vyn i kompakt form. |
| [ShowInOutlineForm](./showinoutlineform/) | Layoutar PivotTable i konturform. |
| [ShowInTabularForm](./showintabularform/) | Layoutar PivotTable i tabellform. |
| [GetCellByDisplayName](./getcellbydisplayname/) | Hämtar Cell-objektet via visningsnamnet för PivotField. |
| [GetDependentPivotTables](./getdependentpivottables/) | Hämtar alla PivotTables som använder denna PivotTable som datakälla. |
| [ExportViewToJson](./exportviewtojson/) | Exporterar pivotsyn som JSON. |
