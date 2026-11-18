---
title: "Cells-klass"
linktitle: "Cells"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Cells-klass. Inkapslar objektet som representerar celler i Go."
type: docs
weight: 200
url: /sv/go-cpp/cells/
---

## Cells class

Inkapslar en samling av cellrelaterade objekt, såsom <see cref="Cell"/>, <see cref="Row"/>, med mera.

```go

type Cells struct  {
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
| [GetOdsCellFields](./getodscellfields/) | Hämtar listan över fält i ods. |
| [Dispose](./dispose/) | Utför applikationsdefinierade uppgifter som är kopplade till frigöring, släppande eller återställning av ohanterade resurser. |
| [GetCount](./getcount/) | Hämtar det totala antalet instanserade Cell-objekt. |
| [GetCountLarge](./getcountlarge/) | Hämtar det totala antalet instanserade Cell-objekt. |
| [GetEnumerator](./getenumerator/) | Hämtar cellernas enumerator. |
| [GetRows](./getrows/) | Hämtar samlingen av Row-objekt som representerar de enskilda raderna i detta kalkylblad. |
| [GetMergedAreas](./getmergedareas/) | Hämtar alla sammanslagna celler. |
| [CheckCell](./checkcell/) | Hämtar Cell-elementet eller null vid angivet radindex och kolumnindex för cellen. |
| [CheckRow](./checkrow/) | Hämtar Row-elementet eller null vid angivet radindex för cellen. |
| [CheckColumn](./checkcolumn/) | Hämtar Column-elementet eller null vid angivet kolumnindex. |
| [IsRowHidden](./isrowhidden/) | Kontrollerar om en rad på angivet index är dold. |
| [IsColumnHidden](./iscolumnhidden/) | Kontrollerar om en kolumn på angivet index är dold. |
| [AddRange](./addrange/) | Lägger till en referens till ett områdeobjekt i celler |
| [CreateRange_String_String](./createrange_string_string/) | Skapar ett Range-objekt från ett område av celler. |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | Skapar ett Range-objekt från ett område av celler. |
| [CreateRange_String](./createrange_string/) | Skapar ett Range-objekt från en adress för området. |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | Skapar ett Range-objekt från rader av celler eller kolumner av celler. |
| [Get_Int_Int](./get_int_int/) | Hämtar Cell-elementet på det angivna cellradindexet och kolumnindexet. |
| [Get_String](./get_string/) | Hämtar Cell-elementet på det angivna cellnamnet. |
| [GetMultiThreadReading](./getmultithreadreading/) | Hämtar eller anger om cellernas datamodell ska stödja flerdelat läsning. Standardvärdet för denna egenskap är false. |
| [SetMultiThreadReading](./setmultithreadreading/) | Hämtar eller anger om cellernas datamodell ska stödja flerdelat läsning. Standardvärdet för denna egenskap är false. |
| [GetMemorySetting](./getmemorysetting/) | Hämtar eller anger minnesanvändningsalternativet för dessa celler. |
| [SetMemorySetting](./setmemorysetting/) | Hämtar eller anger minnesanvändningsalternativet för dessa celler. |
| [Clear](./clear/) | Rensar all data i arbetsbladet. |
| [GetStyle](./getstyle/) | Hämtar och anger standardstilen för arbetsbladet. |
| [SetStyle](./setstyle/) | Hämtar och anger standardstilen för arbetsbladet. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | Hämtar eller anger standardbredden för kolumner i arbetsbladet, i tum. |
| [SetStandardWidthInch](./setstandardwidthinch/) | Hämtar eller anger standardbredden för kolumner i arbetsbladet, i tum. |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | Hämtar eller anger standardbredden för kolumner i arbetsbladet, i pixlar. |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | Hämtar eller anger standardbredden för kolumner i arbetsbladet, i pixlar. |
| [GetStandardWidth](./getstandardwidth/) | Hämtar eller anger standardbredden för kolumner i arbetsbladet, i tecken. |
| [SetStandardWidth](./setstandardwidth/) | Hämtar eller anger standardbredden för kolumner i arbetsbladet, i tecken. |
| [GetStandardHeight](./getstandardheight/) | Hämtar eller anger standardhöjden för rader i detta arbetsblad, i punkter. |
| [SetStandardHeight](./setstandardheight/) | Hämtar eller anger standardhöjden för rader i detta arbetsblad, i punkter. |
| [GetStandardHeightPixels](./getstandardheightpixels/) | Hämtar eller anger standardhöjden för rader i detta arbetsblad, i pixlar. |
| [SetStandardHeightPixels](./setstandardheightpixels/) | Hämtar eller anger standardhöjden för rader i detta arbetsblad, i pixlar. |
| [GetStandardHeightInch](./getstandardheightinch/) | Hämtar eller anger standardhöjden för rader i detta arbetsblad, i tum. |
| [SetStandardHeightInch](./setstandardheightinch/) | Hämtar eller anger standardhöjden för rader i detta arbetsblad, i tum. |
| [ImportFormulaArray](./importformulaarray/) | Importerar en matris av formler till ett arbetsblad. |
| [TextToColumns](./texttocolumns/) | Delar upp innehåll i angiven kolumn i flera kolumner.. |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | Importera en CSV-fil till cellerna. |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | Importera en CSV-fil till cellerna. |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | Importera en CSV-fil till cellerna. |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | Importera en CSV-fil till cellerna. |
| [GetPreserveString](./getpreservestring/) | Hämtar eller anger ett värde som indikerar om alla arbetsbladsvärden bevaras som strängar. Standard är false. |
| [SetPreserveString](./setpreservestring/) | Hämtar eller anger ett värde som indikerar om alla arbetsbladsvärden bevaras som strängar. Standard är false. |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | Slår ihop ett angivet område av celler till en enda cell. |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | Slår ihop ett angivet område av celler till en enda cell. |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | Slår ihop ett angivet område av celler till en enda cell. |
| [UnMerge](./unmerge/) | Delar upp ett angivet område av sammanslagna celler. |
| [ClearMergedCells](./clearmergedcells/) | Rensar alla sammanslagna områden. |
| [HideRow](./hiderow/) | Döljer en rad. |
| [UnhideRow](./unhiderow/) | Visar en rad. |
| [HideRows](./hiderows/) | Döljer flera rader. |
| [UnhideRows](./unhiderows/) | Visar de dolda raderna. |
| [SetRowHeightPixel](./setrowheightpixel/) | Ställer in radhöjd i pixlar. |
| [SetRowHeightInch](./setrowheightinch/) | Ställer in radhöjd i tum. |
| [SetRowHeight](./setrowheight/) | Ställer in höjden på den angivna raden. |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | Hämtar radens höjd. |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | Hämtar kolumnens bredd. |
| [HideColumn](./hidecolumn/) | Döljer en kolumn. |
| [UnhideColumn](./unhidecolumn/) | Visar en kolumn |
| [HideColumns](./hidecolumns/) | Dölj flera kolumner. |
| [UnhideColumns](./unhidecolumns/) | Visa flera kolumner. |
| [GetRowHeight_Int](./getrowheight_int/) | Hämtar höjden på en angiven rad, i enhet punkter. |
| [GetViewRowHeight](./getviewrowheight/) | Hämtar höjden på en angiven rad. |
| [GetRowHeightInch](./getrowheightinch/) | Hämtar höjden på en angiven rad i tum. |
| [GetViewRowHeightInch](./getviewrowheightinch/) | Hämtar höjden på en angiven rad i tum. |
| [GetRowHeightPixel](./getrowheightpixel/) | Hämtar höjden på en angiven rad i pixlar. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Ställer in kolumnbredd i pixlar i normal vy. |
| [SetColumnWidthInch](./setcolumnwidthinch/) | Ställer in kolumnbredd i tum i normal vy. |
| [SetColumnWidth](./setcolumnwidth/) | Ställer in bredden på den angivna kolumnen i normal vy. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Hämtar bredden på den angivna kolumnen i normal vy, i pixelenheter. |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | Hämtar bredden (i tecken) på den angivna kolumnen i normal vy |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | Hämta bredden i olika vystyper. |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | Ställer in kolumnens bredd i olika vyer. |
| [GetMinRow](./getminrow/) | Minsta radindex för cell som innehåller data eller stil. |
| [GetMaxRow](./getmaxrow/) | Största radindex för cell som innehåller data eller stil. |
| [GetMinColumn](./getmincolumn/) | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [GetMaxColumn](./getmaxcolumn/) | Maximalt kolumnindex för de celler som har instansierats i samlingen(inkluderar inte kolumnen där stil är definierad för hela kolumnen men ingen cell har instansierats i den). |
| [GetMinDataRow](./getmindatarow/) | Minsta radindex för cell som innehåller data. |
| [GetMaxDataRow](./getmaxdatarow/) | Maximalt radindex för cell som innehåller data. |
| [GetMinDataColumn](./getmindatacolumn/) | Minsta kolumnindex för cell som innehåller data. |
| [GetMaxDataColumn](./getmaxdatacolumn/) | Maximalt kolumnindex för cell som innehåller data. |
| [GetLastDataRow](./getlastdatarow/) | Hämtar det sista radindexet för cell som innehåller data i den angivna kolumnen. |
| [GetFirstDataRow](./getfirstdatarow/) | Hämtar det första radindexet för cell som innehåller data i den angivna kolumnen. |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Indikerar att radhöjden och standardteckenhöjden matchar |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Indikerar att radhöjden och standardteckenhöjden matchar |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | Indikerar om raden är standarddolt. |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Indikerar om raden är standarddolt. |
| [GetColumns](./getcolumns/) | Hämtar samlingen av Column-objekt som representerar de enskilda kolumnerna i detta kalkylblad. |
| [ApplyColumnStyle](./applycolumnstyle/) | Tillämpar format för en hel kolumn. |
| [ApplyRowStyle](./applyrowstyle/) | Tillämpar format för en hel rad. |
| [ApplyStyle](./applystyle/) | Tillämpar format för ett helt kalkylblad. |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | Kopierar data och format för en hel kolumn. |
| [CopyColumn](./copycolumn/) | Kopierar data och format för en hel kolumn. |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | Kopierar data och format för hela kolumner. |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | Kopierar data och format för de hela kolumnerna. |
| [CopyRow](./copyrow/) | Kopierar data och format för en hel rad. |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | Kopierar data och format för några hela rader. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | Kopierar data och format för några hela rader. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | Kopierar data och format för några hela rader. |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Hämtar konturnivån (nollbaserad) för raden. |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Hämtar konturnivån (nollbaserad) för kolumnen. |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Hämtar den maximala grupperade kolumnens konturnivå (nollbaserad). |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Hämtar den maximala grupperade radens konturnivå (nollbaserad). |
| [ShowGroupDetail](./showgroupdetail/) | Expanderar de grupperade raderna/kolumnerna. |
| [HideGroupDetail](./hidegroupdetail/) | Komprimerar de grupperade raderna/kolumnerna. |
| [UngroupColumns](./ungroupcolumns/) | Avgrupperar kolumner. |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | Grupperar kolumner. |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | Grupperar kolumner. |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | Avgrupperar rader. |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | Avgrupperar rader. |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | Grupperar rader. |
| [GroupRows_Int_Int](./grouprows_int_int/) | Grupperar rader. |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | Tar bort en kolumn. |
| [DeleteColumn_Int](./deletecolumn_int/) | Tar bort en kolumn. |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | Tar bort flera kolumner. |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | Tar bort flera kolumner. |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Kontrollera om området kan tas bort. |
| [DeleteRow_Int](./deleterow_int/) | Tar bort en rad. |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | Tar bort en rad. |
| [DeleteRows_Int_Int](./deleterows_int_int/) | Tar bort flera rader. |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | Tar bort flera rader i kalkylbladet. |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | Tar bort flera rader i kalkylbladet. |
| [DeleteBlankColumns](./deleteblankcolumns/) | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | Ta bort alla tomma kolumner som inte innehåller någon data. |
| [IsBlankColumn](./isblankcolumn/) | Kontrollerar om given kolumn är tom(innehåller ingen data). |
| [DeleteBlankRows](./deleteblankrows/) | Ta bort alla tomma rader som inte innehåller någon data eller annat objekt. |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | Ta bort alla tomma rader som inte innehåller någon data eller vissa speciella objekt såsom synlig kommentar, pivottabell. |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | Infogar några kolumner i kalkylbladet. |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | Infogar några kolumner i kalkylbladet. |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | Infogar en ny kolumn i kalkylbladet. |
| [InsertColumn_Int](./insertcolumn_int/) | Infogar en ny kolumn i kalkylbladet. |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | Infogar flera rader i kalkylbladet. |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | Infogar flera rader i kalkylbladet. |
| [InsertRows_Int_Int](./insertrows_int_int/) | Infogar flera rader i kalkylbladet. |
| [InsertRow](./insertrow/) | Infogar en ny rad i kalkylbladet. |
| [GetRanges](./getranges/) | Hämtar samlingen av Range-objekt som skapats vid körning. |
| [ClearRange_CellArea](./clearrange_cellarea/) | Rensar innehåll och formatering för ett område. |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | Rensar innehåll och formatering för ett område. |
| [ClearContents_CellArea](./clearcontents_cellarea/) | Rensar innehållet i ett område. |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | Rensar innehållet i ett område. |
| [ClearFormats_CellArea](./clearformats_cellarea/) | Rensar formateringen för ett område. |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | Rensar formateringen för ett område. |
| [GetLastCell](./getlastcell/) | Hämtar den sista cellen i detta kalkylblad. |
| [LinkToXmlMap](./linktoxmlmap/) | Länk till en XML-karta. |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | Hämtar det maximala området som inkluderar data, sammanslagna celler och former. |
| [GetFirstCell](./getfirstcell/) | Hämtar den första cellen i detta kalkylblad. |
| [Find_Object_Cell](./find_object_cell/) | Hittar cellen som innehåller inmatningsobjektet. |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | Hittar cellen som innehåller inmatningsobjektet. |
| [EndCellInRow_Int](./endcellinrow_int/) | Hämtar den sista cellen i den här raden. |
| [EndCellInColumn_Int](./endcellincolumn_int/) | Hämtar den sista cellen i den här kolumnen. |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | Hämtar den sista cellen med högsta kolumnindex i detta område. |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | Hämtar den sista cellen med högsta radindex i detta område. |
| [MoveRange](./moverange/) | Flyttar området. |
| [InsertCutCells](./insertcutcells/) | Infoga klippt område. |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | Infogar ett cellområde och förskjuter celler enligt förskjutningsalternativet. |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | Infogar ett cellområde och förskjuter celler enligt förskjutningsalternativet. |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | Infogar ett cellområde och förskjuter celler enligt förskjutningsalternativet. |
| [DeleteRange](./deleterange/) | Raderar ett cellområde och förskjuter celler enligt förskjutningsalternativet. |
| [ExportArray](./exportarray/) | Exporterar data i Cells-samlingen till ett tvådimensionellt array-objekt. |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Hämtar subtotalinställningarna för området. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | Skapar subtotaler för området. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | Skapar subtotaler för området. |
| [RemoveFormulas](./removeformulas/) | Tar bort alla formler och ersätter med formelns värde. |
| [RemoveDuplicates](./removeduplicates/) | Tar bort dubblett rader i bladet. |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | Tar bort dubblettvärden i området. |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | Tar bort dubblettdata i området. |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | Konverterar all strängdata i arbetsbladet till numeriskt värde om möjligt. |
| [GetDependents](./getdependents/) | Hämta alla celler som refererar till den specifika cellen. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Hämtar alla celler vars beräknade resultat beror på en specifik cell. |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | Hämtar alla celler som innehåller inbäddad bild. |
| [GetCellStyle](./getcellstyle/) | Hämta stilen för given cell. |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | Hämta visningsstilen för given cell. |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | Hämta visningsstilen för given cell. |
