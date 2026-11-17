---
title: "Classe Row"
linktitle: "Row"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Row. Incapsula l'oggetto che rappresenta row in Go."
type: docs
weight: 200
url: /it/go-cpp/row/
---

## Row class

Rappresenta una singola riga in un foglio di lavoro.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | Ottieni la cella con indice specifico nella collezione di celle di questa riga. |
| [IsBlank](./isblank/) | Indica se la riga contiene dati |
| [Get](./get/) | Ottiene la cella. |
| [GetEnumerator](./getenumerator/) | Ottiene l'enumeratore delle celle |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Ottiene un enumeratore che itera le celle attraverso questa riga. |
| [GetCellOrNull](./getcellornull/) | Ottiene la cella o null nell'indice specificato. |
| [IsCollapsed](./iscollapsed/) | se la riga è compressa |
| [SetIsCollapsed](./setiscollapsed/) | se la riga è compressa |
| [GetHeight](./getheight/) | Ottiene e imposta l'altezza della riga in unità di punti. |
| [SetHeight](./setheight/) | Ottiene e imposta l'altezza della riga in unità di punti. |
| [IsHidden](./ishidden/) | Indica se la riga è nascosta. |
| [SetIsHidden](./setishidden/) | Indica se la riga è nascosta. |
| [GetIndex](./getindex/) | Restituisce l'indice di questa riga. |
| [GetGroupLevel](./getgrouplevel/) | Restituisce il livello di gruppo della riga. |
| [SetGroupLevel](./setgrouplevel/) | Restituisce il livello di gruppo della riga. |
| [IsHeightMatched](./isheightmatched/) | Indica se l'altezza della riga corrisponde all'impostazione del carattere predefinito corrente della cartella di lavoro. Il valore true di questa proprietà indica anche che l'altezza della riga è "automatico" senza un valore di altezza personalizzato impostato dall'utente. |
| [SetIsHeightMatched](./setisheightmatched/) | Indica se l'altezza della riga corrisponde all'impostazione del carattere predefinito corrente della cartella di lavoro. Il valore true di questa proprietà indica anche che l'altezza della riga è "automatico" senza un valore di altezza personalizzato impostato dall'utente. |
| [GetStyle](./getstyle/) | Restituisce lo stile di questa riga. |
| [SetStyle](./setstyle/) | Imposta lo stile di questa riga. |
| [GetHasCustomStyle](./gethascustomstyle/) | Indica se questa riga ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla cartella di lavoro). |
| [CopySettings](./copysettings/) | Copia le impostazioni della riga, come stile, altezza, visibilità, ...ecc. |
| [GetFirstCell](./getfirstcell/) | Restituisce il primo oggetto cella nella riga. |
| [GetFirstDataCell](./getfirstdatacell/) | Restituisce la prima cella non vuota nella riga. |
| [GetLastCell](./getlastcell/) | Restituisce l'ultimo oggetto cella nella riga. |
| [GetLastDataCell](./getlastdatacell/) | Restituisce l'ultima cella non vuota nella riga. |
| [ApplyStyle](./applystyle/) | Applica formati a un'intera riga. |
| [Equals_Object](./equals_object/) | Verifica se questo oggetto si riferisce alla stessa riga di un altro. |
| [Equals_Row](./equals_row/) | Verifica se questo oggetto si riferisce alla stessa riga di un altro oggetto riga. |
