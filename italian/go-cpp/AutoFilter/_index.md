---
title: "Classe AutoFilter"
linktitle: "AutoFilter"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe AutoFilter. Incapsula l'oggetto che rappresenta l'autofiltro in Go."
type: docs
weight: 200
url: /it/go-cpp/autofilter/
---

## AutoFilter class

Rappresenta l'autofiltro per il foglio di lavoro specificato.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | Ottiene l'ordinatore dei dati. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | Imposta l'intervallo a cui si applica l'AutoFilter specificato. |
| [GetCellArea](./getcellarea/) | Ottiene l'AreaCella dove si applica questo AutoFilter. |
| [GetCellArea_Bool](./getcellarea_bool/) | Ottiene l'Aspose.Cells.CellArea dove si applica l'AutoFilter specificato. |
| [GetRange](./getrange/) | Rappresenta l'intervallo a cui si applica l'AutoFilter specificato. |
| [SetRange_String](./setrange_string/) | Rappresenta l'intervallo a cui si applica l'AutoFilter specificato. |
| [AddFilter](./addfilter/) | Aggiunge un filtro per una colonna di filtro. |
| [AddDateFilter](./adddatefilter/) | Aggiunge un filtro data. |
| [RemoveDateFilter](./removedatefilter/) | Rimuove un filtro data. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | Rimuove un filtro per una colonna di filtro. |
| [Filter](./filter/) | Filtra un elenco con i criteri specificati. |
| [FilterTop10](./filtertop10/) | Filtra i primi 10 elementi dell'elenco |
| [Dynamic_Filter](./dynamic_filter/) | Aggiunge un filtro dinamico. |
| [AddFontColorFilter](./addfontcolorfilter/) | Aggiunge un filtro colore carattere. |
| [AddFillColorFilter](./addfillcolorfilter/) | Aggiunge un filtro colore riempimento. |
| [AddIconFilter](./addiconfilter/) | Aggiunge un filtro icona. |
| [MatchBlanks](./matchblanks/) | Corrisponde a tutte le celle vuote nell'elenco. |
| [MatchNonBlanks](./matchnonblanks/) | Corrisponde a tutte le celle non vuote nell'elenco. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Filtra un elenco con un criterio personalizzato. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Filtra un elenco con criteri personalizzati. |
| [ShowAll](./showall/) | Mostra tutte le righe. |
| [RemoveFilter_Int](./removefilter_int/) | Rimuove il filtro specifico. |
| [Refresh](./refresh/) | Aggiorna i filtri automatici per nascondere o mostrare le righe. |
| [Refresh_Bool](./refresh_bool/) | Ottiene tutti gli indici delle righe nascoste. |
| [GetShowFilterButton](./getshowfilterbutton/) | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [SetShowFilterButton](./setshowfilterbutton/) | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [GetFilterColumns](./getfiltercolumns/) | Ottiene la raccolta delle colonne di filtro. |
