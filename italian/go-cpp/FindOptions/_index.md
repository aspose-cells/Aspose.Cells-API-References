---
title: "FindOptions Class"
linktitle: "FindOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "FindOptions class. Incapsula l'oggetto che rappresenta findoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/findoptions/
---

## FindOptions class

Rappresenta le opzioni di ricerca.

```go

type FindOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewFindOptions](./newfindoptions/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetCaseSensitive](./getcasesensitive/) | Indica se la stringa cercata è sensibile al maiuscolo/minuscolo. |
| [SetCaseSensitive](./setcasesensitive/) | Indica se la stringa cercata è sensibile al maiuscolo/minuscolo. |
| [GetLookAtType](./getlookattype/) | Guarda il tipo. |
| [SetLookAtType](./setlookattype/) | Guarda il tipo. |
| [GetRange](./getrange/) | Ottiene e imposta l'intervallo cercato. |
| [SetRange](./setrange/) | Imposta l'intervallo cercato. |
| [IsRangeSet](./israngeset/) | Indica se l'intervallo cercato è impostato. |
| [GetSearchBackward](./getsearchbackward/) | Se cercare all'indietro per le celle. |
| [SetSearchBackward](./setsearchbackward/) | Se cercare all'indietro per le celle. |
| [GetSearchOrderByRows](./getsearchorderbyrows/) | Indica se l'ordine di ricerca è per righe o colonne. |
| [SetSearchOrderByRows](./setsearchorderbyrows/) | Indica se l'ordine di ricerca è per righe o colonne. |
| [GetLookInType](./getlookintype/) | Guarda nel tipo. |
| [SetLookInType](./setlookintype/) | Guarda nel tipo. |
| [GetRegexKey](./getregexkey/) | Indica se la chiave cercata è una regex.Se vero la chiave cercata sarà considerata come regex e analizzata.Altrimenti la chiave sarà analizzata secondo le regole di MS Excel. |
| [SetRegexKey](./setregexkey/) | Indica se la chiave cercata è una regex.Se vero la chiave cercata sarà considerata come regex e analizzata.Altrimenti la chiave sarà analizzata secondo le regole di MS Excel. |
| [GetValueTypeSensitive](./getvaluetypesensitive/) | Indica se il tipo di valore della cella cercata deve essere lo stesso della chiave cercata. |
| [SetValueTypeSensitive](./setvaluetypesensitive/) | Indica se il tipo di valore della cella cercata deve essere lo stesso della chiave cercata. |
| [GetStyle](./getstyle/) | Il formato da cercare. |
| [SetStyle](./setstyle/) | Il formato da cercare. |
| [GetConvertNumericData](./getconvertnumericdata/) | Ottiene o imposta un valore che indica se convertire il valore stringa cercato in dati numerici. |
| [SetConvertNumericData](./setconvertnumericdata/) | Ottiene o imposta un valore che indica se convertire il valore stringa cercato in dati numerici. |
