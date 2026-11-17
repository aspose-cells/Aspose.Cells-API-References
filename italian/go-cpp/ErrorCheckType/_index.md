---
title: "Enum ErrorCheckType"
linktitle: "ErrorCheckType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Enum ErrorCheckType. Incapsula l'oggetto che rappresenta errorchecktype in Go."
type: docs
weight: 200
url: /it/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

Rappresenta tutti i tipi di controllo errori.

```go

type ErrorCheckType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [EvaluationError](./evaluationerror/) | Ignora gli errori quando le celle contengono formule che generano un errore. |
| [EmptyCellRef](./emptycellref/) | Ignora gli errori quando le formule fanno riferimento a celle vuote. |
| [NumberStoredAsText](./numberstoredastext/) | Ignora gli errori quando i numeri sono formattati come testo o sono preceduti da un apostrofo |
| [InconsistRange](./inconsistrange/) | Ignora gli errori quando le formule omettono alcune celle in una regione. |
| [InconsistFormula](./inconsistformula/) | Ignora gli errori quando una formula in una regione del foglio di lavoro differisce dalle altre formule nella stessa regione. |
| [TwoDigitTextYear](./twodigittextyear/) | Ignora gli errori quando le formule contengono celle formattate come testo con anni rappresentati con 2 cifre. |
| [UnlockedFormula](./unlockedformula/) | Ignora gli errori quando le celle sbloccate contengono formule. |
| [TableDataValidation](./tabledatavalidation/) | Ignora gli errori quando il valore di una cella in una Tabella non rispetta le regole di convalida dei dati specificate. |
| [CalculatedColumn](./calculatedcolumn/) | Ignora gli errori quando le celle contengono un valore diverso dalla formula calcolata della colonna. |
