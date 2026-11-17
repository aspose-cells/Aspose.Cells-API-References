---
title: "Classe Top10"
linktitle: "Top10"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Top10. Incapsula l'oggetto che rappresenta top10 in Go."
type: docs
weight: 200
url: /it/go-cpp/top10/
---

## Top10 class

Descrivi la regola di formattazione condizionale Top10. Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia superiore N o inferiore N, come specificato.

```go

type Top10 struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewTop10](./newtop10/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [IsPercent](./ispercent/) | Ottieni o imposta se una regola "top/bottom n" è una regola "top/bottom n percent". Il valore predefinito è false. |
| [SetIsPercent](./setispercent/) | Ottieni o imposta se una regola "top/bottom n" è una regola "top/bottom n percent". Il valore predefinito è false. |
| [IsBottom](./isbottom/) | Ottieni o imposta se una regola "top/bottom n" è una regola "bottom n". Il valore predefinito è false. |
| [SetIsBottom](./setisbottom/) | Ottieni o imposta se una regola "top/bottom n" è una regola "bottom n". Il valore predefinito è false. |
| [GetRank](./getrank/) | Ottieni o imposta il valore di "n" in una regola di formattazione condizionale "top/bottom n". Se IsPercent è true, il valore deve essere compreso tra 0 e 100. Altrimenti deve essere compreso tra 0 e 1000. Il valore predefinito è 10. |
| [SetRank](./setrank/) | Ottieni o imposta il valore di "n" in una regola di formattazione condizionale "top/bottom n". Se IsPercent è true, il valore deve essere compreso tra 0 e 100. Altrimenti deve essere compreso tra 0 e 1000. Il valore predefinito è 10. |
