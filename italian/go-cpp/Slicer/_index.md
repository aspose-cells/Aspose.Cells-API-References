---
title: "Classe Slicer"
linktitle: "Slicer"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Slicer. Incapsula l'oggetto che rappresenta lo slicer in Go."
type: docs
weight: 200
url: /it/go-cpp/slicer/
---

## Slicer class

descrizione sommaria di Slicer View

```go

type Slicer struct  {
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
| [GetSortOrderType](./getsortordertype/) | Indica il tipo di ordinamento degli elementi. |
| [SetSortOrderType](./setsortordertype/) | Indica il tipo di ordinamento degli elementi. |
| [GetShowMissing](./getshowmissing/) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [SetShowMissing](./setshowmissing/) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | Indica se mostrare gli elementi eliminati dalla fonte dati. |
| [GetShowAllItems](./getshowallitems/) | Indica se mostrare tutti gli elementi anche se non ci sono dati o sono eliminati. Il valore predefinito è true; |
| [SetShowAllItems](./setshowallitems/) | Indica se mostrare tutti gli elementi anche se non ci sono dati o sono eliminati. Il valore predefinito è true; |
| [AddPivotConnection](./addpivotconnection/) | Aggiunge la connessione PivotTable. |
| [RemovePivotConnection](./removepivotconnection/) | Rimuove la connessione PivotTable. |
| [GetLockedPosition](./getlockedposition/) | Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente. |
| [SetLockedPosition](./setlockedposition/) | Indica se lo slicer specificato può essere spostato o ridimensionato tramite l'interfaccia utente. |
| [Refresh](./refresh/) | Aggiornamento degli elementi dello slicer dalle tabelle pivot associate. |
| [GetShape](./getshape/) | Restituisce l'oggetto Shape associato allo slicer specificato. Sola lettura. |
| [GetSlicerCache](./getslicercache/) | Restituisce l'oggetto SlicerCache associato allo slicer. Sola lettura. |
| [GetWorksheet](./getworksheet/) | Restituisce l'oggetto Worksheet che contiene questo slicer. Sola lettura. |
| [GetStyleType](./getstyletype/) | Specifica il tipo di stile slicer incorporato. Il tipo predefinito è SlicerStyleLight1. |
| [SetStyleType](./setstyletype/) | Specifica il tipo di stile slicer incorporato. Il tipo predefinito è SlicerStyleLight1. |
| [GetName](./getname/) | Restituisce o imposta il nome dello slicer specificato |
| [SetName](./setname/) | Restituisce o imposta il nome dello slicer specificato |
| [GetCaption](./getcaption/) | Restituisce o imposta la didascalia dello slicer specificato. |
| [SetCaption](./setcaption/) | Restituisce o imposta la didascalia dello slicer specificato. |
| [GetFirstItemIndex](./getfirstitemindex/) | Specifica l'indice basato su zero del primo elemento dello slicer. |
| [SetFirstItemIndex](./setfirstitemindex/) | Specifica l'indice basato su zero del primo elemento dello slicer. |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | Rimuovi le etichette filtro selezionate. |
| [ClearFilter](./clearfilter/) | Rimuovi filtri |
| [GetShowCaption](./getshowcaption/) | Indica se l'intestazione dello slicer è visibile. Il valore predefinito è true |
| [SetShowCaption](./setshowcaption/) | Indica se l'intestazione dello slicer è visibile. Il valore predefinito è true |
| [GetNumberOfColumns](./getnumberofcolumns/) | Restituisce o imposta il numero di colonne nello slicer. Il valore predefinito è 1. |
| [SetNumberOfColumns](./setnumberofcolumns/) | Restituisce o imposta il numero di colonne nello slicer. Il valore predefinito è 1. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Ottiene o imposta la larghezza di ogni colonna nello slicer, in unità di pixel. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Ottiene o imposta la larghezza di ogni colonna nello slicer, in unità di pixel. |
| [GetColumnWidth](./getcolumnwidth/) | Restituisce o imposta la larghezza di ogni colonna nello slicer in unità di punti. |
| [SetColumnWidth](./setcolumnwidth/) | Restituisce o imposta la larghezza di ogni colonna nello slicer in unità di punti. |
| [GetRowHeightPixel](./getrowheightpixel/) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato, in unità di pixel. |
| [SetRowHeightPixel](./setrowheightpixel/) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato, in unità di pixel. |
| [GetRowHeight](./getrowheight/) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti. |
| [SetRowHeight](./setrowheight/) | Restituisce o imposta l'altezza di ogni riga nello slicer specificato in unità di punti. |
