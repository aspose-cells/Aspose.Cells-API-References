---
title: "Arbetsbladsklass"
linktitle: "Arbetsblad"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Arbetsbladsklass. Inkapslar objektet som representerar ett arbetsblad i Go."
type: docs
weight: 200
url: /sv/go-cpp/worksheet/
---

## Worksheet class

Inkapslar objektet som representerar ett enskilt arbetsblad.

```go

type Worksheet struct  {
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
| [GetProtection](./getprotection/) | Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett arbetsblad. Stöder avancerade skyddsalternativ i ExcelXP och senare versioner. |
| [GetUniqueId](./getuniqueid/) | Hämtar och anger det unika ID:t, det är samma som {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId](./setuniqueid/) | Hämtar och anger det unika ID:t, det är samma som {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetPanes](./getpanes/) | Hämtar fönsterpanelerna. |
| [GetWorkbook](./getworkbook/) | Hämtar arbetsboksobjektet som innehåller detta blad. |
| [GetCells](./getcells/) | Hämtar Aspose.Cells.Cells‑samlingen. |
| [GetQueryTables](./getquerytables/) | Hämtar QueryTableCollection i arbetsbladet. |
| [GetType](./gettype/) | Representerar arbetsbladstyp. |
| [SetType](./settype/) | Representerar arbetsbladstyp. |
| [GetName](./getname/) | Hämtar eller anger namnet på arbetsbladet. |
| [SetName](./setname/) | Hämtar eller anger namnet på arbetsbladet. |
| [GetShowFormulas](./getshowformulas/) | Anger om formler eller deras resultat ska visas. |
| [SetShowFormulas](./setshowformulas/) | Anger om formler eller deras resultat ska visas. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | Anger om ikoner för datatyper ska visas. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | Anger om ikoner för datatyper ska visas. |
| [IsGridlinesVisible](./isgridlinesvisible/) | Hämtar eller anger ett värde som indikerar om rutnätslinjerna är synliga.Default är true. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | Hämtar eller anger ett värde som indikerar om rutnätslinjerna är synliga.Default är true. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Hämtar eller anger ett värde som indikerar om arbetsbladet ska visa rad- och kolumnrubriker.Default är true. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Hämtar eller anger ett värde som indikerar om arbetsbladet ska visa rad- och kolumnrubriker.Default är true. |
| [GetPaneState](./getpanestate/) | Anger om panelen har horisontella eller vertikala delningar, och om dessa delningar är frysta. |
| [GetDisplayZeros](./getdisplayzeros/) | Sant om nollvärden visas. |
| [SetDisplayZeros](./setdisplayzeros/) | Sant om nollvärden visas. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | Anger om det angivna arbetsbladet visas från höger till vänster istället för från vänster till höger.Standard är falskt. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | Anger om det angivna arbetsbladet visas från höger till vänster istället för från vänster till höger.Standard är falskt. |
| [IsOutlineShown](./isoutlineshown/) | Anger om konturen ska visas. |
| [SetIsOutlineShown](./setisoutlineshown/) | Anger om konturen ska visas. |
| [IsSelected](./isselected/) | Anger om detta arbetsblad är markerat när arbetsboken öppnas. |
| [SetIsSelected](./setisselected/) | Anger om detta arbetsblad är markerat när arbetsboken öppnas. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Fryser rutor vid den angivna cellen i arbetsbladet. |
| [GetFreezedPanes](./getfreezedpanes/) | Hämtar de frysta rutorna. |
| [Split](./split/) | Delar fönstret. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Fryser rutor vid den angivna cellen i arbetsbladet. |
| [UnFreezePanes](./unfreezepanes/) | Låser upp rutor i arbetsbladet. |
| [RemoveSplit](./removesplit/) | Tar bort delat fönster. |
| [GetPivotTables](./getpivottables/) | Hämtar alla pivottabeller i detta arbetsblad. |
| [GetListObjects](./getlistobjects/) | Hämtar alla ListObjects i detta arbetsblad. |
| [GetTabId](./gettabid/) | Anger det interna identifieraren för bladet. |
| [SetTabId](./settabid/) | Anger det interna identifieraren för bladet. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Hämtar samlingen HorizontalPageBreakCollection. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | Hämtar samlingen VerticalPageBreakCollection. |
| [AddPageBreaks](./addpagebreaks/) | Lägger till sidbrytning. |
| [GetHyperlinks](./gethyperlinks/) | Hämtar samlingen HyperlinkCollection. |
| [Copy_Worksheet](./copy_worksheet/) | Kopierar innehåll och format från ett annat arbetsblad. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Kopierar innehåll och format från ett annat arbetsblad. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Anpassar automatiskt kolumnbredden. |
| [AutoFitColumns](./autofitcolumns/) | Anpassar automatiskt alla kolumner i detta arbetsblad. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Anpassar automatiskt alla kolumner i detta arbetsblad. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | Anpassar automatiskt kolumnbredden. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Anpassar automatiskt kolumnernas bredd. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Anpassar automatiskt kolumnernas bredd. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Anpassar automatiskt kolumnernas bredd. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Anpassar automatiskt kolumnernas bredd. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Anpassar automatiskt radhöjden. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Anpassar automatiskt radhöjden. |
| [AutoFitRows](./autofitrows/) | Anpassar automatiskt alla rader i detta arbetsblad. |
| [AutoFitRows_Bool](./autofitrows_bool/) | Anpassar automatiskt alla rader i detta arbetsblad. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Anpassar automatiskt alla rader i detta arbetsblad. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | Anpassar automatiskt radhöjden i ett område. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Anpassar automatiskt radhöjden i ett område. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Anpassar automatiskt radhöjden i ett rektangulärt område. |
| [AutoFitRow_Int](./autofitrow_int/) | Anpassar automatiskt radhöjden. |
| [GetPageSetup](./getpagesetup/) | Representerar sidinställningsbeskrivningen i detta blad. |
| [GetAutoFilter](./getautofilter/) | Representerar autofilter för det angivna arbetsbladet. |
| [Filter](./filter/) | Filtrerar intervallet. |
| [GetAdvancedFilter](./getadvancedfilter/) | Hämtar inställningarna för avancerat filter. |
| [Advanced_Filter](./advanced_filter/) | Filtrerar data med komplexa kriterier. |
| [RemoveAutoFilter](./removeautofilter/) | Tar bort autofiltret för kalkylbladet. |
| [GetHasAutofilter](./gethasautofilter/) | Anger om detta kalkylblad har autofilter. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | Anger om alternativet för övergångsformelutvärdering (Lotus‑kompatibilitet) är aktiverat. |
| [SetTransitionEvaluation](./settransitionevaluation/) | Anger om alternativet för övergångsformelutvärdering (Lotus‑kompatibilitet) är aktiverat. |
| [GetTransitionEntry](./gettransitionentry/) | Anger om alternativet för övergångsformelinmatning (Lotus‑kompatibilitet) är aktiverat. |
| [SetTransitionEntry](./settransitionentry/) | Anger om alternativet för övergångsformelinmatning (Lotus‑kompatibilitet) är aktiverat. |
| [GetVisibilityType](./getvisibilitytype/) | Anger det synliga tillståndet för detta blad. |
| [SetVisibilityType](./setvisibilitytype/) | Anger det synliga tillståndet för detta blad. |
| [SetVisible](./setvisible/) | Ställer in de synliga alternativen. |
| [IsVisible](./isvisible/) | Representerar om kalkylbladet är synligt. |
| [SetIsVisible](./setisvisible/) | Representerar om kalkylbladet är synligt. |
| [SelectRange](./selectrange/) | Markerar ett intervall. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | Tar bort alla ritobjekt i detta kalkylblad. |
| [ClearComments](./clearcomments/) | Rensar alla kommentarer i designerns kalkylblad. |
| [GetSparklineGroups](./getsparklinegroups/) | Hämtar sparkline-grupperna i kalkylbladet. |
| [GetCharts](./getcharts/) | Hämtar en diagramsamling |
| [GetComments](./getcomments/) | Hämtar kommentarsamlingen. |
| [GetPictures](./getpictures/) | Hämtar en bildsamling. |
| [GetAllPictures](./getallpictures/) | Hämtar alla bilder, inklusive bilder som är inbäddade i cellen och över cellerna. |
| [GetTextBoxes](./gettextboxes/) | Hämtar en textrutansamling. |
| [GetCheckBoxes](./getcheckboxes/) | Hämtar en kryssrutan-samling. |
| [GetOleObjects](./getoleobjects/) | Representerar en samling av OleObject i ett kalkylblad. |
| [GetShapes](./getshapes/) | Returnerar alla ritformer i detta kalkylblad. |
| [GetSlicers](./getslicers/) | Hämta slicer‑samlingen i kalkylbladet |
| [GetTimelines](./gettimelines/) | Hämta tidslinje‑samlingen i kalkylbladet |
| [Protect_ProtectionType](./protect_protectiontype/) | Skyddar kalkylbladet. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Skyddar kalkylbladet. |
| [Unprotect](./unprotect/) | Avskyddar arbetsbladet. |
| [Unprotect_String](./unprotect_string/) | Avskyddar arbetsbladet. |
| [GetIndex](./getindex/) | Hämtar indexet för bladet i arbetsbladsamlingen. |
| [MoveTo](./moveto/) | Flyttar bladet till en annan plats i kalkylarket. |
| [IsProtected](./isprotected/) | Indikerar om arbetsbladet är skyddat. |
| [GetValidations](./getvalidations/) | Hämtar samlingen av datavalideringsinställningar i arbetsbladet. |
| [GetAllowEditRanges](./getalloweditranges/) | Hämtar samlingen av tillåtna redigeringsområden i arbetsbladet. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | Hämtar felkontrollinställning som tillämpas på vissa områden. |
| [GetOutline](./getoutline/) | Hämtar konturen i detta arbetsblad. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | Representerar det första synliga radindexet. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | Representerar det första synliga radindexet. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | Representerar det första synliga kolumnindexet. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | Representerar det första synliga kolumnindexet. |
| [Replace](./replace/) | Ersätter all cellers text med en ny sträng. |
| [GetZoom](./getzoom/) | Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400. |
| [SetZoom](./setzoom/) | Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400. |
| [GetViewType](./getviewtype/) | Hämtar och anger vytypen. |
| [SetViewType](./setviewtype/) | Hämtar och anger vytypen. |
| [IsPageBreakPreview](./ispagebreakpreview/) | Indikerar om det angivna arbetsbladet visas i normal vy eller sidbrytningförhandsgranskning. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | Indikerar om det angivna arbetsbladet visas i normal vy eller sidbrytningförhandsgranskning. |
| [IsRulerVisible](./isrulervisible/) | Indikerar om linjalen är synlig. Denna egenskap gäller endast för sidbrytningförhandsgranskning. |
| [SetIsRulerVisible](./setisrulervisible/) | Indikerar om linjalen är synlig. Denna egenskap gäller endast för sidbrytningförhandsgranskning. |
| [GetSelectedAreas](./getselectedareas/) | Hämtar valda cellområden i designerns kalkylark. |
| [GetTabColor](./gettabcolor/) | Representerar flikfärgen för arbetsbladet. |
| [SetTabColor](./settabcolor/) | Representerar flikfärgen för arbetsbladet. |
| [GetGridlineColor](./getgridlinecolor/) | Hämtar och anger färgen på rutnätslinjen. |
| [SetGridlineColor](./setgridlinecolor/) | Hämtar och anger färgen på rutnätslinjen. |
| [GetCodeName](./getcodename/) | Hämtar arbetsbladets kodnamn. |
| [SetCodeName](./setcodename/) | Hämtar arbetsbladets kodnamn. |
| [GetBackgroundImage](./getbackgroundimage/) | Hämtar och anger arbetsbladets bakgrundsbild. |
| [SetBackgroundImage](./setbackgroundimage/) | Hämtar och anger arbetsbladets bakgrundsbild. |
| [GetConditionalFormattings](./getconditionalformattings/) | Hämtar de villkorliga formateringarna i arbetsbladet. |
| [GetActiveCell](./getactivecell/) | Hämtar eller anger den aktiva cellen i arbetsbladet. |
| [SetActiveCell](./setactivecell/) | Hämtar eller anger den aktiva cellen i arbetsbladet. |
| [GetCustomProperties](./getcustomproperties/) | Hämtar ett objekt som representerar identifieringsinformationen som är associerad med ett arbetsblad. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | Hämtar automatiska sidbrytningar. |
| [GetSmartTagSetting](./getsmarttagsetting/) | Hämtar alla SmartTagCollection-objekt i arbetsbladet. |
| [ToString](./tostring/) | Returnerar en sträng som representerar det aktuella Worksheet-objektet. |
| [GetScenarios](./getscenarios/) | Hämtar samlingen av Scenario. |
| [StartAccessCache](./startaccesscache/) | Startar sessionen som använder cache för att komma åt data i detta worksheet. |
| [CloseAccessCache](./closeaccesscache/) | Stänger sessionen som använder cache för att komma åt data i detta worksheet. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Konverterar formelreferensstilen. |
| [CalculateFormula_String](./calculateformula_string/) | Beräknar en formel. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Beräknar ett formeluttryck direkt. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Beräknar ett formeluttryck direkt. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Beräknar en formel som matrisformel. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Beräknar en formel som matrisformel. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Beräknar en formel som matrisformel. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Beräknar alla formler i detta worksheet. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | Fråga cellområden som är mappade/länkade till den specifika sökvägen för xml map. |
| [GetCellWatches](./getcellwatches/) | Hämtar samling av celler i detta worksheet som övervakas i 'watch window'. |
| [RefreshPivotTables](./refreshpivottables/) | Uppdaterar alla PivotTables i detta Worksheet. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Uppdaterar alla PivotTables i detta Worksheet. |
