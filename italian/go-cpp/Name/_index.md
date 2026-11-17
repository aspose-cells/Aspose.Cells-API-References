---
title: "Name Classe"
linktitle: "Name"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Name classe. Incapsula l'oggetto che rappresenta name in Go."
type: docs
weight: 200
url: /it/go-cpp/name/
---

## Name class

Rappresenta un nome definito per un intervallo di celle.

```go

type Name struct  {
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
| [GetComment](./getcomment/) | Ottiene e imposta il commento del nome. Solo per Excel 2007 o versioni successive. |
| [SetComment](./setcomment/) | Ottiene e imposta il commento del nome. Solo per Excel 2007 o versioni successive. |
| [GetText](./gettext/) | Ottiene il testo del nome dell'oggetto. |
| [SetText](./settext/) | Ottiene il testo del nome dell'oggetto. |
| [GetFullText](./getfulltext/) | Ottiene il testo completo del nome dell'oggetto con l'impostazione di ambito. |
| [GetRefersTo](./getrefersto/) | Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con un segno di uguale. |
| [SetRefersTo_String](./setrefersto_string/) | Restituisce o imposta la formula a cui il nome è definito per fare riferimento, iniziando con un segno di uguale. |
| [GetR1C1RefersTo](./getr1c1refersto/) | Ottiene o imposta un riferimento R1C1 del Nome. |
| [SetR1C1RefersTo](./setr1c1refersto/) | Ottiene o imposta un riferimento R1C1 del Nome. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Ottieni il riferimento di questo Nome. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Ottieni il riferimento di questo Nome basato sulla cella specificata. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Imposta il riferimento di questo Nome. |
| [IsReferred](./isreferred/) | Indica se questo nome è referenziato da altre formule. |
| [IsVisible](./isvisible/) | Indica se il nome è visibile. |
| [SetIsVisible](./setisvisible/) | Indica se il nome è visibile. |
| [GetSheetIndex](./getsheetindex/) | Indica se questo nome appartiene a Cartella di lavoro o Foglio di lavoro. 0 = Nome globale, altrimenti indice al foglio (basato su 1). |
| [SetSheetIndex](./setsheetindex/) | Indica se questo nome appartiene a Cartella di lavoro o Foglio di lavoro. 0 = Nome globale, altrimenti indice al foglio (basato su 1). |
| [ToString](./tostring/) | Restituisce una stringa che rappresenta l'oggetto Range corrente. |
| [GetRanges](./getranges/) | Ottiene tutti gli intervalli referenziati da questo nome. |
| [GetRanges_Bool](./getranges_bool/) | Ottiene tutti gli intervalli referenziati da questo nome. |
| [GetReferredAreas](./getreferredareas/) | Ottiene tutti i riferimenti referenziati da questo nome. |
| [GetRange](./getrange/) | Ottiene l'intervallo se questo nome fa riferimento a un intervallo. |
| [GetRange_Bool](./getrange_bool/) | Ottiene l'intervallo se questo nome fa riferimento a un intervallo |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | Ottiene l'intervallo se questo nome fa riferimento a un intervallo. Se il riferimento di questo nome non è assoluto, l'intervallo può variare per celle diverse. |
