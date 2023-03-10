---
title: FormatConditionType enumerazione
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 2100
url: /it/python-net/aspose.cells/formatconditiontype/
is_root: false
---
##  FormatConditionType enumerazione
Tipo di regola di formato condizionale.



Il tipo FormatConditionType espone i membri seguenti:

###  Campi
| Campo| Descrizione|
| :- | :- |
| CELL_VALUE | Questa regola di formattazione condizionale confronta un valore di cella<br/> a un risultato calcolato da una formula, utilizzando un operatore.|
| EXPRESSION | Questa regola di formattazione condizionale contiene una formula per<br/>valutare. Quando il risultato della formula è vero, la cella lo è<br/> evidenziato.|
| COLOR_SCALE | Questa regola di formattazione condizionale crea un file graduato<br/> scala di colori sulle celle.|
| DATA_BAR | Questa regola di formattazione condizionale visualizza un file graduato<br/> barra dei dati nell'intervallo di celle.|
| ICON_SET |Questa regola di formattazione condizionale applica le icone alle celle<br/> secondo i loro valori.|
| TOP10 | Questa regola di formattazione condizionale evidenzia le celle cui<br/>i valori rientrano nella parentesi N superiore o N inferiore, come<br/> specificato.|
| UNIQUE_VALUES | Questa regola di formattazione condizionale evidenzia unique<br/> valori nell'intervallo.|
| DUPLICATE_VALUES | Questa regola di formattazione condizionale evidenzia i duplicati<br/> valori.|
| CONTAINS_TEXT | Questa regola di formattazione condizionale evidenzia le celle<br/>contenente un determinato testo. Equivalente all'utilizzo di SEARCH()<br/>funzione foglio per determinare se la cella contiene<br/> il testo.|
| NOT_CONTAINS_TEXT | Questa regola di formattazione condizionale evidenzia le celle che<br/>non contengono il testo specificato. Equivalente all'utilizzo di SEARCH()<br/>funzione foglio per determinare se la cella contiene<br/> il testo oppure no.|
| BEGINS_WITH | Questa regola di formattazione condizionale evidenzia le celle nel file<br/>intervallo che inizia con il testo dato. Equivalente a<br/> utilizzando la funzione foglio LEFT() e confrontando i valori.|
| ENDS_WITH | Questa regola di formattazione condizionale evidenzia le celle che terminano<br/>con il testo dato. Equivale all'utilizzo del foglio RIGHT()<br/> funzione e confronto dei valori.|
| CONTAINS_BLANKS | Questa regola di formattazione condizionale evidenzia le celle che<br/>sono completamente vuote. Equivalente all'utilizzo di LEN(TRIM()).<br/>Ciò significa che se la cella contiene solo caratteri<br/>che TRIM() rimuoverebbe, allora è considerato vuoto.<br/> Anche una cella vuota è considerata vuota.|
| NOT_CONTAINS_BLANKS | Questa regola di formattazione condizionale evidenzia le celle che<br/>non sono vuoti. Equivalente all'utilizzo di LEN(TRIM()). Questo<br/>significa che se la cella contiene solo caratteri che<br/>TRIM() verrebbe rimosso, quindi è considerato vuoto. UN<br/> anche la cella vuota è considerata vuota.|
| CONTAINS_ERRORS | Questa regola di formattazione condizionale evidenzia le celle con<br/>errori di formula Equivalente all'utilizzo del foglio ISERROR()<br/> funzione per determinare se c'è un errore di formula.|
| NOT_CONTAINS_ERRORS | Questa regola di formattazione condizionale evidenzia le celle<br/>senza errori di formula. Equivalente all'uso di ISERROR()<br/> funzione foglio per determinare se c'è un errore di formula.|
| TIME_PERIOD | Questa regola di formattazione condizionale evidenzia le celle<br/>contenenti date nel periodo di tempo specificato. IL<br/>viene valutato il valore sottostante della cella, quindi il<br/>cella non deve essere formattata come una data da essere<br/>valutato. Ad esempio, con una cella contenente il file<br/>valore 38913 il formato condizionale deve essere applicato se<br/> la regola richiede un valore di 7/14/2006.|
| ABOVE_AVERAGE | Questa regola di formattazione condizionale evidenzia le celle che<br/>sono al di sopra o al di sotto della media per tutti i valori in<br/> allineare.|



###  Guarda anche
* modulo [aspose.cells](..)
