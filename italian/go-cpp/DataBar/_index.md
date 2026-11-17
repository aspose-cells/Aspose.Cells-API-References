---
title: "Classe DataBar"
linktitle: "DataBar"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe DataBar. Incapsula l'oggetto che rappresenta databar in Go."
type: docs
weight: 200
url: /it/go-cpp/databar/
---

## DataBar class

Descrivi la regola di formattazione condizionale DataBar.Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle.

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dei dati. |
| [SetAxisColor](./setaxiscolor/) | Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dei dati. |
| [GetAxisPosition](./getaxisposition/) | Ottiene o imposta la posizione dell'asse delle barre dei dati specificate da una regola di formattazione condizionale. |
| [SetAxisPosition](./setaxisposition/) | Ottiene o imposta la posizione dell'asse delle barre dei dati specificate da una regola di formattazione condizionale. |
| [GetBarFillType](./getbarfilltype/) | Ottiene o imposta come una barra dei dati è riempita di colore. |
| [SetBarFillType](./setbarfilltype/) | Ottiene o imposta come una barra dei dati è riempita di colore. |
| [GetDirection](./getdirection/) | Ottiene o imposta la direzione in cui la barra dei dati è visualizzata. |
| [SetDirection](./setdirection/) | Ottiene o imposta la direzione in cui la barra dei dati è visualizzata. |
| [GetBarBorder](./getbarborder/) | Ottiene un oggetto che specifica il bordo di una barra dei dati. |
| [GetNegativeBarFormat](./getnegativebarformat/) | Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale della barra dei dati. |
| [GetMinCfvo](./getmincfvo/) | Ottieni o imposta l'oggetto valore minimo di questa DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max. |
| [GetMaxCfvo](./getmaxcfvo/) | Ottieni o imposta l'oggetto valore massimo di questa DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Min. |
| [GetColor](./getcolor/) | Ottieni o imposta il colore di questa DataBar. |
| [SetColor](./setcolor/) | Ottieni o imposta il colore di questa DataBar. |
| [GetMinLength](./getminlength/) | Rappresenta la lunghezza minima della barra dei dati. |
| [SetMinLength](./setminlength/) | Rappresenta la lunghezza minima della barra dei dati. |
| [GetMaxLength](./getmaxlength/) | Rappresenta la lunghezza massima della barra dei dati. |
| [SetMaxLength](./setmaxlength/) | Rappresenta la lunghezza massima della barra dei dati. |
| [GetShowValue](./getshowvalue/) | Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicata questa barra dei dati. Il valore predefinito è true. |
| [SetShowValue](./setshowvalue/) | Ottieni o imposta il flag che indica se mostrare i valori delle celle a cui è applicata questa barra dei dati. Il valore predefinito è true. |
| [ToImage](./toimage/) | Renderizza la barra dei dati nella cella in un array di byte dell'immagine. |
