---
title: "CustomDocumentPropertyCollection Classe"
linktitle: "CustomDocumentPropertyCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "CustomDocumentPropertyCollection class. Incapsula l'oggetto che rappresenta customdocumentpropertycollection in Go."
type: docs
weight: 200
url: /it/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

Una raccolta di proprietà del documento personalizzate.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [Add_String_String](./add_string_string/) | Crea una nuova proprietà documento personalizzata del tipo di dati <b>PropertyType.String</b>. |
| [Add_String_Int](./add_string_int/) | Crea una nuova proprietà documento personalizzata del tipo di dati <b>PropertyType.Number</b>. |
| [Add_String_Date](./add_string_date/) | Crea una nuova proprietà documento personalizzata del tipo di dati <b>PropertyType.DateTime</b>. |
| [Add_String_Bool](./add_string_bool/) | Crea una nuova proprietà documento personalizzata del tipo di dati <b>PropertyType.Boolean</b>. |
| [Add_String_Double](./add_string_double/) | Crea una nuova proprietà documento personalizzata del tipo di dati <b>PropertyType.Float</b>. |
| [AddLinkToContent](./addlinktocontent/) | Crea una nuova proprietà documento personalizzata che si collega al contenuto. |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Aggiorna i valori di tutte le proprietà personalizzate collegate al contenuto (usecell value of linked range to update value of custom property). |
| [UpdateLinkedRange](./updatelinkedrange/) | Aggiorna tutti gli intervalli collegati alle proprietà personalizzate (use the value ofcustom document property to update cell value of linked range). |
| [Get_Int](./get_int/) | Restituisce un oggetto DocumentProperty per indice. |
| [Contains](./contains/) | Restituisce true se una proprietà con il nome specificato esiste nella collezione. |
| [IndexOf](./indexof/) | Ottiene l'indice di una proprietà per nome. |
| [Remove](./remove/) | Rimuove una proprietà con il nome specificato dalla collezione. |
| [RemoveAt](./removeat/) | Rimuove una proprietà all'indice specificato. |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
