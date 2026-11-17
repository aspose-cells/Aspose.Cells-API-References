---
title: "PivotTableCollection Classe"
linktitle: "PivotTableCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "PivotTableCollection classe. Incapsula l'oggetto che rappresenta pivottablecollection in Go."
type: docs
weight: 200
url: /it/go-cpp/pivottablecollection/
---

## PivotTableCollection class

Rappresenta la raccolta di tutti gli oggetti PivotTable nel foglio di lavoro specificato.

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino delle risorse non gestite. |
| [Add_String_Int_Int](./add_string_int_int/) | Aggiunge una nuova PivotTable nella riga e colonna del foglio di lavoro specificate con le opzioni predefinite. |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003. |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | Aggiunge una nuova PivotTable. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Aggiunge una nuova PivotTable basata su un'altra PivotTable. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Aggiunge una nuova PivotTable basata su un'altra PivotTable. |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | Aggiunge un nuovo oggetto PivotTable alla collezione con più intervalli di consolidamento come origine dati. |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | Aggiunge un nuovo oggetto PivotTable alla collezione con più intervalli di consolidamento come origine dati. |
| [Get_Int](./get_int/) | Ottiene il report della PivotTable per indice. |
| [Get_String](./get_string/) | Ottiene il report della PivotTable per nome della PivotTable. |
| [Get_Int_Int](./get_int_int/) | Ottiene il report della PivotTable per posizione della PivotTable. |
| [Clear](./clear/) | Cancella tutte le pivot table. |
| [Remove_PivotTable](./remove_pivottable/) | Elimina la PivotTable specificata e rimuove i dati della PivotTable. |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | Elimina la PivotTable specificata. |
| [RemoveAt_Int](./removeat_int/) | Elimina la PivotTable all'indice specificato e rimuove i dati della PivotTable. |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | Elimina la PivotTable all'indice specificato. |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
