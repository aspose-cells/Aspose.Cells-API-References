---
title: "Classe ColorScale"
linktitle: "ColorScale"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ColorScale. Incapsula l'oggetto che rappresenta colorscale in Go."
type: docs
weight: 200
url: /it/go-cpp/colorscale/
---

## ColorScale class

Descrivi la regola di formattazione condizionale ColorScale.Questa regola di formattazione condizionale crea una scala di colori graduale sulle celle.

```go

type ColorScale struct  {
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
| [GetIs3ColorScale](./getis3colorscale/) | Indica se la formattazione condizionale è a scala di 3 colori. |
| [SetIs3ColorScale](./setis3colorscale/) | Indica se la formattazione condizionale è a scala di 3 colori. |
| [GetMinCfvo](./getmincfvo/) | Ottieni o imposta l'oggetto valore minimo di questa ColorScale. Impossibile impostare null o CFValueObject con tipo FormatConditionValueType.Max su di esso. |
| [GetMidCfvo](./getmidcfvo/) | Ottieni o imposta l'oggetto valore medio di questa ColorScale. Impossibile impostare CFValueObject con tipo FormatConditionValueType.Max o FormatConditionValueType.Min su di esso. |
| [GetMaxCfvo](./getmaxcfvo/) | Ottieni o imposta l'oggetto valore massimo di questa ColorScale. Impossibile impostare null o CFValueObject con tipo FormatConditionValueType.Min su di esso. |
| [GetMinColor](./getmincolor/) | Ottieni o imposta il colore gradiente per il valore minimo nell'intervallo. |
| [SetMinColor](./setmincolor/) | Ottieni o imposta il colore gradiente per il valore minimo nell'intervallo. |
| [GetMidColor](./getmidcolor/) | Ottieni o imposta il colore gradiente per il valore medio nell'intervallo. |
| [SetMidColor](./setmidcolor/) | Ottieni o imposta il colore gradiente per il valore medio nell'intervallo. |
| [GetMaxColor](./getmaxcolor/) | Ottieni o imposta il colore gradiente per il valore massimo nell'intervallo. |
| [SetMaxColor](./setmaxcolor/) | Ottieni o imposta il colore gradiente per il valore massimo nell'intervallo. |
