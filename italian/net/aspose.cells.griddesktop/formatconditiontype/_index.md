---
title: "Enum FormatConditionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridDesktop.FormatConditionType enum. Tipo di regola di formattazione condizionale"
type: docs
url: /it/net/aspose.cells.griddesktop/formatconditiontype/
---
## FormatConditionType enumeration

Tipo di regola di formattazione condizionale.

```csharp
public enum FormatConditionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| CellValue | `0` | Questa regola di formattazione condizionale confronta il valore di una cella con il risultato calcolato di una formula, utilizzando un operatore. |
| Expression | `1` | Questa regola di formattazione condizionale contiene una formula da valutare. Quando il risultato della formula è vero, la cella viene evidenziata. |
| ColorScale | `2` | Questa regola di formattazione condizionale crea una scala di colori graduale sulle celle. |
| DataBar | `3` | Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle. |
| IconSet | `4` | Questa regola di formattazione condizionale applica icone alle celle in base ai loro valori. |
| Top10 | `5` | Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia superiore N o inferiore N, come specificato. |
| UniqueValues | `6` | Questa regola di formattazione condizionale evidenzia i valori unici nell'intervallo. |
| DuplicateValues | `7` | Questa regola di formattazione condizionale evidenzia i valori duplicati. |
| ContainsText | `8` | Questa regola di formattazione condizionale evidenzia le celle che contengono il testo specificato. Equivalente all'uso della funzione foglio SEARCH() per determinare se la cella contiene il testo. |
| NotContainsText | `9` | Questa regola di formattazione condizionale evidenzia le celle che non sono vuote. Equivalente all'uso di LEN(TRIM()). Ciò significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, viene considerata vuota. Anche una cella vuota è considerata vuota. |
| BeginsWith | `10` | Questa regola di formattazione condizionale evidenzia le celle nell'intervallo che iniziano con il testo specificato. Equivalente all'uso della funzione foglio LEFT() e al confronto dei valori. |
| EndsWith | `11` | Questa regola di formattazione condizionale evidenzia le celle che terminano con il testo specificato. Equivalente all'uso della funzione foglio RIGHT() e al confronto dei valori. |
| ContainsBlanks | `12` | Questa regola di formattazione condizionale evidenzia le celle completamente vuote. Equivalente all'uso di LEN(TRIM()). Ciò significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, viene considerata vuota. Anche una cella vuota è considerata vuota. |
| NotContainsBlanks | `13` | Questa regola di formattazione condizionale evidenzia le celle che non sono vuote. Equivalente all'uso di LEN(TRIM()). Ciò significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, viene considerata vuota. Anche una cella vuota è considerata vuota. |
| ContainsErrors | `14` | Questa regola di formattazione condizionale evidenzia le celle con errori di formula. Equivalente all'uso della funzione foglio ISERROR() per determinare se c'è un errore di formula. |
| NotContainsErrors | `15` | Questa regola di formattazione condizionale evidenzia le celle senza errori di formula. Equivalente all'uso della funzione foglio ISERROR() per determinare se c'è un errore di formula. |
| TimePeriod | `16` | Questa regola di formattazione condizionale evidenzia le celle contenenti date nel periodo di tempo specificato. Il valore sottostante della cella viene valutato, quindi la cella non deve essere formattata come data per essere valutata. Ad esempio, con una cella contenente il valore 38913 la formattazione condizionale verrà applicata se la regola richiede un valore di 7/14/2006. |
| AboveAverage | `17` | Questa regola di formattazione condizionale evidenzia le celle che sono sopra o sotto la media per tutti i valori nell'intervallo. |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


