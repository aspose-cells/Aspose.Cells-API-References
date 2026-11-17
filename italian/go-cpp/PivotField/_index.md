---
title: "PivotField Class"
linktitle: "PivotField"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "PivotField class. Incapsula l'oggetto che rappresenta pivotfield in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotfield/
---

## PivotField class

Rappresenta un campo in un report di PivotTable.

```go

type PivotField struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetPivotItems](./getpivotitems/) | Ottiene gli elementi pivot del campo pivot |
| [GetMaxValue](./getmaxvalue/) | Ottiene il valore massimo di questo campo. |
| [GetMinValue](./getminvalue/) | Ottiene il valore massimo di questo campo. |
| [GetGroupSettings](./getgroupsettings/) | Ottiene le impostazioni di gruppo del campo pivot. |
| [InitPivotItems](./initpivotitems/) | Inizializza gli elementi pivot del campo pivot |
| [Group](./group/) | Raggruppa automaticamente il campo. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Raggruppa il campo pivot con opzioni. |
| [GroupBy](./groupby/) | Raggruppa manualmente il campo. |
| [Ungroup](./ungroup/) | Annulla il raggruppamento del campo pivot. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | Ottiene il filtro pivot del campo pivot per tipo |
| [GetFilters](./getfilters/) | Ottiene tutti i filtri pivot applicati a questo campo pivot. |
| [ClearFilter](./clearfilter/) | Cancella l'impostazione del filtro su questo campo pivot. |
| [FilterTop10](./filtertop10/) | Filtra per valori del campo pivot dei dati. |
| [FilterByValue](./filterbyvalue/) | Filtra per valori del campo pivot dei dati. |
| [FilterByLabel](./filterbylabel/) | Filtra per didascalie del campo pivot di riga o colonna. |
| [FilterByDate](./filterbydate/) | Filtra per valori di data del campo pivot di riga o colonna. |
| [IsCalculatedField](./iscalculatedfield/) | Indica se questo campo pivot è un campo calcolato. |
| [GetFormula](./getformula/) | Ottiene la formula del campo calcolato. Funziona solo per i campi calcolati. |
| [IsValuesField](./isvaluesfield/) | Indica se questo campo rappresenta il campo valori. |
| [GetBaseIndex](./getbaseindex/) | Rappresenta l'indice nei campi pivot di origine. |
| [SetBaseIndex](./setbaseindex/) | Rappresenta l'indice nei campi pivot di origine. |
| [GetPosition](./getposition/) | Rappresenta l'indice del PivotField nella regione. |
| [GetRegionType](./getregiontype/) | Specifica la regione della tabella pivot in cui questo campo è visualizzato. |
| [GetName](./getname/) | Rappresenta il nome del PivotField. |
| [SetName](./setname/) | Rappresenta il nome del PivotField. |
| [GetDisplayName](./getdisplayname/) | Rappresenta il nome visualizzato del campo pivot nella visualizzazione della tabella pivot. |
| [SetDisplayName](./setdisplayname/) | Rappresenta il nome visualizzato del campo pivot nella visualizzazione della tabella pivot. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Imposta come calcolare i subtotali per il campo specificato. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Indica se mostrare il subtotale specificato per questo campo pivot. |
| [GetSubtotals](./getsubtotals/) | Ottiene o imposta i subtotali del campo. Solo per i campi pivot di riga o colonna. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Ottiene o imposta i subtotali del campo. Solo per i campi pivot di riga o colonna. |
| [IsAutoSubtotals](./isautosubtotals/) | Indica se il campo specificato mostra subtotali automatici. Il valore predefinito è true. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | Indica se il campo specificato mostra subtotali automatici. Il valore predefinito è true. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | Indica se il campo specificato può essere trascinato nella regione di riga. Il valore predefinito è true. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | Indica se il campo specificato può essere trascinato nella regione di riga. Il valore predefinito è true. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Indica se il campo specificato può essere trascinato nella regione di colonna. Il valore predefinito è true. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Indica se il campo specificato può essere trascinato nella regione di colonna. Il valore predefinito è true. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | Indica se il campo specificato può essere trascinato nella regione di pagina. Il valore predefinito è true. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | Indica se il campo specificato può essere trascinato nella regione di pagina. Il valore predefinito è true. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. Il valore predefinito è true. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | Indica se questo campo pivot può essere rimosso dalla visualizzazione della PivotTable. Il valore predefinito è true. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | Indica se il campo specificato può essere trascinato nella regione dei valori. Il valore predefinito è true. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | Indica se il campo specificato può essere trascinato nella regione dei valori. Il valore predefinito è true. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Indica se più elementi possono essere selezionati nel campo di pagina. Il valore predefinito è false. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Indica se più elementi possono essere selezionati nel campo di pagina. Il valore predefinito è false. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | Indica se ripetere le etichette del campo nella regione. Il valore predefinito è false. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Indica se ripetere le etichette del campo nella regione. Il valore predefinito è false. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Indica se includere nuovi elementi nel campo nel filtro manuale. Il valore predefinito è false. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Indica se includere nuovi elementi nel campo nel filtro manuale. Il valore predefinito è false. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Indica se inserire interruzioni di pagina dopo ogni elemento. Il valore predefinito è false. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Indica se inserire interruzioni di pagina dopo ogni elemento. Il valore predefinito è false. |
| [GetShowAllItems](./getshowallitems/) | Indica se visualizzare tutti gli elementi nella visualizzazione PivotTable, anche se non contengono dati di riepilogo. Il valore predefinito è false. |
| [SetShowAllItems](./setshowallitems/) | Indica se visualizzare tutti gli elementi nella visualizzazione PivotTable, anche se non contengono dati di riepilogo. Il valore predefinito è false. |
| [SortBy_SortOrder](./sortby_sortorder/) | Ordina questo campo pivot. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Ordina questo campo pivot. |
| [GetSortSetting](./getsortsetting/) | Ottiene tutte le impostazioni dell'ordinamento automatico |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Ottiene le impostazioni Top 10 AutoShow per un campo pivot. |
| [Top10AutoShow](./top10autoshow/) | Configura le impostazioni Top10 AutoShow per questo campo pivot. |
| [GetFunction](./getfunction/) | Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable. |
| [SetFunction](./setfunction/) | Rappresenta la funzione utilizzata per riepilogare questo campo dati della PivotTable. |
| [ShowValuesAs](./showvaluesas/) | Mostra i valori del campo dati in un formato di visualizzazione diverso quando è in uso il calcolo ShowDataAs. |
| [GetShowValuesSetting](./getshowvaluessetting/) | Ottiene le impostazioni per la visualizzazione dei valori quando è in uso il calcolo ShowDataAs. |
| [GetCurrentPageItem](./getcurrentpageitem/) | Rappresenta l'elemento di pagina attualmente selezionato del campo pagina per filtrare i dati. Valido solo per i campi pagina. |
| [SetCurrentPageItem](./setcurrentpageitem/) | Rappresenta l'elemento di pagina attualmente selezionato del campo pagina per filtrare i dati. Valido solo per i campi pagina. |
| [GetInsertBlankRow](./getinsertblankrow/) | Indica se inserire una riga vuota dopo ogni elemento. Valido solo per i campi riga. |
| [SetInsertBlankRow](./setinsertblankrow/) | Indica se inserire una riga vuota dopo ogni elemento. Valido solo per i campi riga. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | Indica se visualizzare i subtotali in cima o in fondo agli elementi quando ShowInOutlineForm è true, quindi |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | Indica se visualizzare i subtotali in cima o in fondo agli elementi quando ShowInOutlineForm è true, quindi |
| [GetShowInOutlineForm](./getshowinoutlineform/) | Indica se disporre questo campo in forma di contorno nella visualizzazione Pivot Table. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | Indica se disporre questo campo in forma di contorno nella visualizzazione Pivot Table. |
| [GetNumber](./getnumber/) | Rappresenta il formato di visualizzazione predefinito di numeri e date. |
| [SetNumber](./setnumber/) | Rappresenta il formato di visualizzazione predefinito di numeri e date. |
| [Get_NumberFormat](./get_numberformat/) | Rappresenta il formato di visualizzazione personalizzato di numeri e date. |
| [SetNumberFormat](./setnumberformat/) | Rappresenta il formato di visualizzazione personalizzato di numeri e date. |
| [HideAllDetails](./hidealldetails/) | Nasconde tutti i dettagli |
| [ShowAllDetails](./showalldetails/) | Mostra tutti i dettagli |
| [GetItems](./getitems/) | Ottieni tutte le etichette degli elementi pivot in questo campo. |
| [GetOriginalItems](./getoriginalitems/) | Ottieni gli elementi base originali; |
| [AddCalculatedItem](./addcalculateditem/) | Aggiungi un elemento formula calcolata al campo pivot. |
| [GetShowCompact](./getshowcompact/) | Indica se visualizzare le etichette del campo successivo nella stessa colonna nella visualizzazione Pivot Table |
| [SetShowCompact](./setshowcompact/) | Indica se visualizzare le etichette del campo successivo nella stessa colonna nella visualizzazione Pivot Table |
