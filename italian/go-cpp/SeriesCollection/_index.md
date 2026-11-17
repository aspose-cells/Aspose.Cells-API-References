---
title: "SeriesCollection Classe"
linktitle: "SeriesCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "SeriesCollection classe. Incapsula l'oggetto che rappresenta seriescollection in Go."
type: docs
weight: 200
url: /it/go-cpp/seriescollection/
---

## SeriesCollection class

Incapsula una raccolta di oggetti <see cref=\"Series\"/>.

```go

type SeriesCollection struct  {
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
| [Get](./get/) | Ottiene l'elemento Series all'indice specificato. |
| [GetSeriesByOrder](./getseriesbyorder/) | Ottiene l'elemento Series per ordine. |
| [RemoveAt](./removeat/) | Rimuove una serie all'indice specifico. |
| [GetCategoryData](./getcategorydata/) | Ottiene o imposta l'intervallo dei valori dell'asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10") o una sequenza di valori (ad esempio "{2,6,8,10}"). |
| [SetCategoryData](./setcategorydata/) | Ottiene o imposta l'intervallo dei valori dell'asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10") o una sequenza di valori (ad esempio "{2,6,8,10}"). |
| [GetSecondCategoryData](./getsecondcategorydata/) | Ottiene o imposta l'intervallo dei valori del secondo asse di categoria. Può essere un intervallo di celle (ad esempio, "d1:e10"), o una sequenza di valori (ad esempio, "{2,6,8,10}"). Ha effetto solo quando alcune serie sono state tracciate sul secondo asse. |
| [SetSecondCategoryData](./setsecondcategorydata/) | Ottiene o imposta l'intervallo dei valori del secondo asse di categoria. Può essere un intervallo di celle (ad esempio, "d1:e10"), o una sequenza di valori (ad esempio, "{2,6,8,10}"). Ha effetto solo quando alcune serie sono state tracciate sul secondo asse. |
| [SwapSeries](./swapseries/) | Modifica direttamente gli ordini delle due serie. |
| [SetSeriesNames](./setseriesnames/) | Imposta i nomi di tutte le serie nel grafico. |
| [AddR1C1](./addr1c1/) | Aggiunge la collezione Series a un grafico. |
| [Add_String_Bool](./add_string_bool/) | Aggiunge la collezione Series a un grafico. |
| [Add_String_Bool_Bool](./add_string_bool_bool/) | Aggiunge la collezione Series a un grafico. |
| [IsColorVaried](./iscolorvaried/) | Rappresenta se il colore dei punti è variabile. |
| [SetIsColorVaried](./setiscolorvaried/) | Rappresenta se il colore dei punti è variabile. |
| [Clear](./clear/) | Cancella la collezione |
| [ChangeColors](./changecolors/) | Imposta la palette monocromatica per le serie del grafico. |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
