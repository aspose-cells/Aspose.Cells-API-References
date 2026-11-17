---
title: "NameCollection Classe"
linktitle: "NameCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "NameCollection classe. Incapsula l'oggetto che rappresenta namecollection in Go."
type: docs
weight: 200
url: /it/go-cpp/namecollection/
---

## NameCollection class

Rappresenta una raccolta di tutti gli oggetti <see cref=\"Name\"/> nel foglio di calcolo.

```go

type NameCollection struct  {
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
| [Add](./add/) | Definisce un nuovo nome. |
| [Get_Int](./get_int/) | Restituisce l'elemento Name all'indice specificato. |
| [Filter](./filter/) | Restituisce tutti i nomi definiti per ambito. |
| [Get_String](./get_string/) | Restituisce l'elemento Name con il nome specificato. |
| [Remove_stringArray](./remove_stringarray/) | Rimuove un array di nomi |
| [Remove_String](./remove_string/) | Rimuove il nome. |
| [RemoveAt](./removeat/) | Rimuove il nome all'indice specifico. |
| [Clear](./clear/) | Rimuove tutti i nomi definiti che non sono referenziati dalle formule e dalla fonte dati. Se il nome definito è referenziato, impostiamo solo Name.ReferTo a null e lo nascondiamo. |
| [RemoveDuplicateNames](./removeduplicatenames/) | Rimuove i nomi definiti duplicati |
| [Sort](./sort/) | Ordina i nomi definiti. |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
