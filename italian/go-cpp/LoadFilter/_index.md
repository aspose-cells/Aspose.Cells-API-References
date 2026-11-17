---
title: "Classe LoadFilter"
linktitle: "LoadFilter"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe LoadFilter. Incapsula l'oggetto che rappresenta loadfilter in Go."
type: docs
weight: 200
url: /it/go-cpp/loadfilter/
---

## LoadFilter class

Rappresenta il filtro che fornisce opzioni per il caricamento dei dati quando si carica la cartella di lavoro da un modello.

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | Crea un LoadFilter con le opzioni di filtro predefinite LoadDataFilterOptions::All. |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Crea un LoadFilter con le opzioni di filtro fornite. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Ottiene le opzioni di filtro per indicare quali dati devono essere caricati. |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Imposta le opzioni di filtro per indicare quali dati devono essere caricati. |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | Specifica i fogli (indici) e l'ordine da caricare. Il valore predefinito è null, il che indica di caricare tutti i fogli nell'ordine predefinito nel file modello. Se non è null e l'indice di qualche foglio non è presente nell'array restituito, allora il foglio non verrà caricato. |
| [StartSheet](./startsheet/) | Prepara le opzioni di filtro prima di caricare il foglio di lavoro specificato. L'implementazione dell'utente di LoadFilter può modificare le LoadDataFilterOptions per indicare come caricare i dati per questo foglio di lavoro. |
