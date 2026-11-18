---
title: "PivotField klass"
linktitle: "PivotField"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotField-klass. Inkapslar objektet som representerar pivotfield i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotfield/
---

## PivotField class

Representerar ett fält i en PivotTable-rapport.

```go

type PivotField struct  {
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
| [GetPivotItems](./getpivotitems/) | Hämtar pivot‑objekten för pivotfältet |
| [GetMaxValue](./getmaxvalue/) | Hämtar maxvärdet för detta fält. |
| [GetMinValue](./getminvalue/) | Hämtar maxvärdet för detta fält. |
| [GetGroupSettings](./getgroupsettings/) | Hämtar gruppinställningarna för pivotfältet. |
| [InitPivotItems](./initpivotitems/) | Initiera pivot‑objekten för pivotfältet |
| [Group](./group/) | Grupperar fältet automatiskt. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Grupperar pivotfältet med alternativ. |
| [GroupBy](./groupby/) | Anpassa gruppering av fältet. |
| [Ungroup](./ungroup/) | Avgruppera pivotfältet. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | Hämtar pivot‑filtret för pivotfältet efter typ. |
| [GetFilters](./getfilters/) | Hämtar alla pivot‑filter som tillämpats för detta pivotfält. |
| [ClearFilter](./clearfilter/) | Rensar filterinställningarna för detta pivotfält. |
| [FilterTop10](./filtertop10/) | Filtrerar efter värden i datapivotfältet. |
| [FilterByValue](./filterbyvalue/) | Filtrerar efter värden i datapivotfältet. |
| [FilterByLabel](./filterbylabel/) | Filtrerar efter rubriker i rad- eller kolumnpivotfältet. |
| [FilterByDate](./filterbydate/) | Filtrerar efter datumvärden för rad- eller kolumnpivotfältet. |
| [IsCalculatedField](./iscalculatedfield/) | Anger om detta pivotfält är ett beräknat fält. |
| [GetFormula](./getformula/) | Hämtar formeln för det beräknade fältet. Fungerar endast för beräknade fält. |
| [IsValuesField](./isvaluesfield/) | Anger om detta fält representerar värdefältet. |
| [GetBaseIndex](./getbaseindex/) | Representerar indexet i källpivotfälten. |
| [SetBaseIndex](./setbaseindex/) | Representerar indexet i källpivotfälten. |
| [GetPosition](./getposition/) | Representerar indexet för PivotField i regionen. |
| [GetRegionType](./getregiontype/) | Anger regionen i pivottabellen där detta fält visas. |
| [GetName](./getname/) | Representerar namnet på PivotField. |
| [SetName](./setname/) | Representerar namnet på PivotField. |
| [GetDisplayName](./getdisplayname/) | Representerar visningsnamnet för pivotfältet i pivottabellvyn. |
| [SetDisplayName](./setdisplayname/) | Representerar visningsnamnet för pivotfältet i pivottabellvyn. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Ställer in hur det angivna fältet ska summeras. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Anger om den angivna delsummeringen ska visas för detta pivotfält. |
| [GetSubtotals](./getsubtotals/) | Hämtar eller anger delsummeringarna för fältet. Endast för rad- eller kolumnpivotfält. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Hämtar eller anger delsummeringarna för fältet. Endast för rad- eller kolumnpivotfält. |
| [IsAutoSubtotals](./isautosubtotals/) | Indikerar om det angivna fältet visar automatiska delsummer. Standard är sant. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | Indikerar om det angivna fältet visar automatiska delsummer. Standard är sant. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | Indikerar om det angivna fältet kan dras till radregionen.Standardvärdet är sant. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | Indikerar om det angivna fältet kan dras till radregionen.Standardvärdet är sant. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Indikerar om det angivna fältet kan dras till kolumnregionen.Standardvärdet är sant. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Indikerar om det angivna fältet kan dras till kolumnregionen.Standardvärdet är sant. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | Indikerar om det angivna fältet kan dras till sidregionen.Standardvärdet är sant. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | Indikerar om det angivna fältet kan dras till sidregionen.Standardvärdet är sant. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | Indikerar om detta pivåfält kan tas bort från PivotTable-vyn.Standardvärdet är sant. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | Indikerar om detta pivåfält kan tas bort från PivotTable-vyn.Standardvärdet är sant. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | Indikerar om det angivna fältet kan dras till värdeområdet.Standardvärdet är sant. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | Indikerar om det angivna fältet kan dras till värdeområdet.Standardvärdet är sant. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Indikerar om flera objekt kan väljas i sidfältet.Standardvärdet är falskt. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Indikerar om flera objekt kan väljas i sidfältet.Standardvärdet är falskt. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | Indikerar om etiketter för fältet ska upprepas i regionen.Standardvärdet är falskt. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Indikerar om etiketter för fältet ska upprepas i regionen.Standardvärdet är falskt. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Indikerar om nya objekt ska inkluderas i fältet i manuellt filter.Standardvärdet är falskt. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Indikerar om nya objekt ska inkluderas i fältet i manuellt filter.Standardvärdet är falskt. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Indikerar om sidbrytningar ska infogas efter varje objekt.Standardvärdet är falskt. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Indikerar om sidbrytningar ska infogas efter varje objekt.Standardvärdet är falskt. |
| [GetShowAllItems](./getshowallitems/) | Indikerar om alla objekt ska visas i PivotTable-vyn,även om de inte innehåller sammanfattningsdata.Standardvärdet är falskt. |
| [SetShowAllItems](./setshowallitems/) | Indikerar om alla objekt ska visas i PivotTable-vyn,även om de inte innehåller sammanfattningsdata.Standardvärdet är falskt. |
| [SortBy_SortOrder](./sortby_sortorder/) | Sorterar detta pivåfält. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Sorterar detta pivåfält. |
| [GetSortSetting](./getsortsetting/) | Hämtar alla inställningar för automatisk sortering |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Hämtar Top 10 AutoShow-inställningarna för ett pivåfält. |
| [Top10AutoShow](./top10autoshow/) | Konfigurerar Top10 AutoShow-inställningarna för detta pivåfält. |
| [GetFunction](./getfunction/) | Representerar funktionen som används för att sammanfatta detta PivotTable-datfält. |
| [SetFunction](./setfunction/) | Representerar funktionen som används för att sammanfatta detta PivotTable-datfält. |
| [ShowValuesAs](./showvaluesas/) | Visar värden för datfältet i olika visningsformat när ShowDataAs-beräkningen är i bruk. |
| [GetShowValuesSetting](./getshowvaluessetting/) | Hämtar inställningarna för att visa värden när ShowDataAs-beräkningen är i bruk. |
| [GetCurrentPageItem](./getcurrentpageitem/) | Representerar det aktuellt valda sidobjektet i sidfältet för att filtrera data.Endast giltigt för sidfält. |
| [SetCurrentPageItem](./setcurrentpageitem/) | Representerar det aktuellt valda sidobjektet i sidfältet för att filtrera data.Endast giltigt för sidfält. |
| [GetInsertBlankRow](./getinsertblankrow/) | Indikerar om en tom rad ska infogas efter varje objekt.Endast för radfält. |
| [SetInsertBlankRow](./setinsertblankrow/) | Indikerar om en tom rad ska infogas efter varje objekt.Endast för radfält. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | Indikerar om delsummer ska visas högst upp eller längst ner på objekt när ShowInOutlineForm är sant, sedan |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | Indikerar om delsummer ska visas högst upp eller längst ner på objekt när ShowInOutlineForm är sant, sedan |
| [GetShowInOutlineForm](./getshowinoutlineform/) | Indikerar om detta fält ska läggas ut i konturform i Pivot Table-vyn. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | Indikerar om detta fält ska läggas ut i konturform i Pivot Table-vyn. |
| [GetNumber](./getnumber/) | Representerar det inbyggda visningsformatet för tal och datum. |
| [SetNumber](./setnumber/) | Representerar det inbyggda visningsformatet för tal och datum. |
| [Get_NumberFormat](./get_numberformat/) | Representerar det anpassade visningsformatet för tal och datum. |
| [SetNumberFormat](./setnumberformat/) | Representerar det anpassade visningsformatet för tal och datum. |
| [HideAllDetails](./hidealldetails/) | Döljer alla detaljer |
| [ShowAllDetails](./showalldetails/) | Visa alla detaljer |
| [GetItems](./getitems/) | Hämta alla etiketter för pivotelement i detta fält. |
| [GetOriginalItems](./getoriginalitems/) | Hämta de ursprungliga basobjekten; |
| [AddCalculatedItem](./addcalculateditem/) | Lägg till ett beräknat formelobjekt i pivotfältet. |
| [GetShowCompact](./getshowcompact/) | Anger om etiketter för nästa fält ska visas i samma kolumn i pivottabellvyn |
| [SetShowCompact](./setshowcompact/) | Anger om etiketter för nästa fält ska visas i samma kolumn i pivottabellvyn |
