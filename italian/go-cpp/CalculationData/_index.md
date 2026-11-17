---
title: "Classe CalculationData"
linktitle: "CalculationData"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe CalculationData. Incapsula l'oggetto che rappresenta calculationdata in Go."
type: docs
weight: 200
url: /it/go-cpp/calculationdata/
---

## CalculationData class

Rappresenta i dati richiesti durante il calcolo di una funzione, come il nome della funzione, i parametri, ...ecc.

```go

type CalculationData struct  {
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
| [GetCalculatedValue](./getcalculatedvalue/) | Ottiene o imposta il valore calcolato per questa funzione. |
| [SetCalculatedValue](./setcalculatedvalue/) | Ottiene o imposta il valore calcolato per questa funzione. |
| [GetWorkbook](./getworkbook/) | Ottiene l'oggetto Workbook in cui si trova la funzione. |
| [GetWorksheet](./getworksheet/) | Ottiene l'oggetto Worksheet in cui si trova la funzione. |
| [GetCellRow](./getcellrow/) | Ottiene l'indice di riga della cella in cui si trova la funzione. |
| [GetCellColumn](./getcellcolumn/) | Ottiene l'indice di colonna della cella in cui si trova la funzione. |
| [GetCell](./getcell/) | Ottiene l'oggetto Cell in cui si trova la funzione. |
| [GetFunctionName](./getfunctionname/) | Ottiene il nome della funzione da calcolare. |
| [GetParamCount](./getparamcount/) | Ottiene il conteggio dei parametri |
| [GetParamValue](./getparamvalue/) | Ottiene l'oggetto valore rappresentato del parametro a un dato indice. |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | Ottiene il valore(i) del parametro a un dato indice. Se il parametro è una sorta di espressione che necessita di essere calcolata, verrà calcolata in modalità array. |
| [GetParamText](./getparamtext/) | Ottiene il testo letterale del parametro all'indice specificato. |
