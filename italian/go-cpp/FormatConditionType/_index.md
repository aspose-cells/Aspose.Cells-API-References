---
title: "Enum FormatConditionType"
linktitle: "FormatConditionType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Enum FormatConditionType. Incapsula l'oggetto che rappresenta formatconditiontype in Go."
type: docs
weight: 200
url: /it/go-cpp/formatconditiontype/
---

## FormatConditionType Enum

Tipo di regola di formattazione condizionale.

```go

type FormatConditionType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [CellValue](./cellvalue/) | Questa regola di formattazione condizionale confronta il valore di una cella con il risultato calcolato da una formula, usando un operatore. |
| [Expression](./expression/) | Questa regola di formattazione condizionale contiene una formula da valutare. Quando il risultato della formula è vero, la cella viene evidenziata. |
| [Top10](./top10/) | Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia superiore N o inferiore N, come specificato. |
| [UniqueValues](./uniquevalues/) | Questa regola di formattazione condizionale evidenzia i valori unici nell'intervallo. |
| [DuplicateValues](./duplicatevalues/) | Questa regola di formattazione condizionale evidenzia i valori duplicati. |
| [ContainsText](./containstext/) | Questa regola di formattazione condizionale evidenzia le celle contenenti il testo specificato. Equivalente all'uso della funzione foglio SEARCH() per determinare se la cella contiene il testo. |
| [NotContainsText](./notcontainstext/) | Questa regola di formattazione condizionale evidenzia le celle che non contengono il testo specificato. Equivalente all'uso della funzione foglio SEARCH() per determinare se la cella contiene o meno il testo. |
| [BeginsWith](./beginswith/) | Questa regola di formattazione condizionale evidenzia le celle nell'intervallo che iniziano con il testo specificato. Equivalente all'uso della funzione foglio LEFT() e al confronto dei valori. |
| [EndsWith](./endswith/) | Questa regola di formattazione condizionale evidenzia le celle che terminano con il testo specificato. Equivalente all'uso della funzione foglio RIGHT() e al confronto dei valori. |
| [ContainsBlanks](./containsblanks/) | Questa regola di formattazione condizionale evidenzia le celle che sono completamente vuote. Equivalente all'uso di LEN(TRIM()). Questo significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, allora è considerata vuota. Una cella vuota è considerata vuota. |
| [NotContainsBlanks](./notcontainsblanks/) | Questa regola di formattazione condizionale evidenzia le celle che non sono vuote. Equivalente all'uso di LEN(TRIM()). Questo significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, allora è considerata vuota. Una cella vuota è considerata vuota. |
| [ContainsErrors](./containserrors/) | Questa regola di formattazione condizionale evidenzia le celle con errori di formula. Equivalente all'uso della funzione foglio ISERROR() per determinare se c'è un errore di formula. |
| [NotContainsErrors](./notcontainserrors/) | Questa regola di formattazione condizionale evidenzia le celle senza errori di formula. Equivalente all'uso della funzione foglio ISERROR() per determinare se c'è un errore di formula. |
| [TimePeriod](./timeperiod/) | Questa regola di formattazione condizionale evidenzia le celle contenenti date nel periodo di tempo specificato. Il valore sottostante della cella viene valutato, quindi la cella non deve essere formattata come data per essere valutata. Ad esempio, con una cella contenente il valore 38913, il formato condizionale verrà applicato se la regola richiede un valore di 14/07/2006. |
| [AboveAverage](./aboveaverage/) | Questa regola di formattazione condizionale evidenzia le celle che sono sopra o sotto la media di tutti i valori nell'intervallo. |
| [ColorScale](./colorscale/) | Questa regola di formattazione condizionale crea una scala gradatedcolor sulle celle. |
| [DataBar](./databar/) | Questa regola di formattazione condizionale visualizza una barra gradateddata nell'intervallo di celle. |
| [IconSet](./iconset/) | Questa regola di formattazione condizionale applica icone alle celle secondo i loro valori. |
