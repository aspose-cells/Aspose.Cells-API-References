---
title: "FormatConditionType"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Tipo di regola di formattazione condizionale."
type: docs
url: /it/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

Tipo di regola di formattazione condizionale.
## Campi

| Campo | Descrizione |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | Questa regola di formattazione condizionale evidenzia le celle che sono al di sopra o al di sotto della media per tutti i valori nell'intervallo. |
| [BEGINS_WITH](#BEGINS-WITH) | Questa regola di formattazione condizionale evidenzia le celle nell'intervallo che iniziano con il testo fornito. |
| [CELL_VALUE](#CELL-VALUE) | Questa regola di formattazione condizionale confronta il valore di una cella con il risultato calcolato da una formula, utilizzando un operatore. |
| [COLOR_SCALE](#COLOR-SCALE) | Questa regola di formattazione condizionale crea una scala di colori graduale sulle celle. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | Questa regola di formattazione condizionale evidenzia le celle che sono completamente vuote. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | Questa regola di formattazione condizionale evidenzia le celle con errori di formula. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | Questa regola di formattazione condizionale evidenzia le celle contenenti il testo fornito. |
| [DATA_BAR](#DATA-BAR) | Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | Questa regola di formattazione condizionale evidenzia i valori duplicati. |
| [ENDS_WITH](#ENDS-WITH) | Questa regola di formattazione condizionale evidenzia le celle che terminano con il testo fornito. |
| [EXPRESSION](#EXPRESSION) | Questa regola di formattazione condizionale contiene una formula da valutare. |
| [ICON_SET](#ICON-SET) | Questa regola di formattazione condizionale applica icone alle celle in base ai loro valori. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | Questa regola di formattazione condizionale evidenzia le celle che non sono vuote. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | Questa regola di formattazione condizionale evidenzia le celle senza errori di formula. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | Questa regola di formattazione condizionale evidenzia le celle che non contengono il testo fornito. |
| [TIME_PERIOD](#TIME-PERIOD) | Questa regola di formattazione condizionale evidenzia le celle contenenti date nel periodo di tempo specificato. |
| [TOP_10](#TOP-10) | Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia dei primi N o degli ultimi N, come specificato. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | Questa regola di formattazione condizionale evidenzia i valori unici nell'intervallo. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


Questa regola di formattazione condizionale evidenzia le celle che sono al di sopra o al di sotto della media per tutti i valori nell'intervallo.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


Questa regola di formattazione condizionale evidenzia le celle nell'intervallo che iniziano con il testo fornito. Equivalente all'uso della funzione foglio LEFT() e al confronto dei valori.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Questa regola di formattazione condizionale confronta il valore di una cella con il risultato calcolato da una formula, utilizzando un operatore.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


Questa regola di formattazione condizionale crea una scala di colori graduale sulle celle.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


Questa regola di formattazione condizionale evidenzia le celle che sono completamente vuote. Equivalente all'uso di LEN(TRIM()). Ciò significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, allora è considerata vuota. Anche una cella vuota è considerata vuota.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


Questa regola di formattazione condizionale evidenzia le celle con errori di formula. Equivalente all'uso della funzione foglio ISERROR() per determinare se c'è un errore di formula.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


Questa regola di formattazione condizionale evidenzia le celle contenenti il testo fornito. Equivalente all'uso della funzione foglio SEARCH() per determinare se la cella contiene il testo.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


Questa regola di formattazione condizionale evidenzia i valori duplicati.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


Questa regola di formattazione condizionale evidenzia le celle che terminano con il testo fornito. Equivalente all'uso della funzione foglio RIGHT() e al confronto dei valori.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


Questa regola di formattazione condizionale contiene una formula da valutare. Quando il risultato della formula è vero, la cella viene evidenziata.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


Questa regola di formattazione condizionale applica icone alle celle in base ai loro valori.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


Questa regola di formattazione condizionale evidenzia le celle che non sono vuote. Equivalente all'uso di LEN(TRIM()). Ciò significa che se la cella contiene solo caratteri che TRIM() rimuoverebbe, allora è considerata vuota. Anche una cella vuota è considerata vuota.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


Questa regola di formattazione condizionale evidenzia le celle senza errori di formula. Equivalente all'uso della funzione di foglio ISERROR() per determinare se esiste un errore di formula.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


Questa regola di formattazione condizionale evidenzia le celle che non contengono il testo specificato. Equivalente all'uso della funzione di foglio SEARCH() per determinare se la cella contiene il testo o meno.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


Questa regola di formattazione condizionale evidenzia le celle contenenti date nel periodo di tempo specificato. Il valore sottostante della cella viene valutato, quindi la cella non deve essere formattata come data per essere valutata. Ad esempio, con una cella contenente il valore 38913, il formato condizionale verrà applicato se la regola richiede un valore di 7/14/2006.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


Questa regola di formattazione condizionale evidenzia le celle i cui valori rientrano nella fascia dei primi N o degli ultimi N, come specificato.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


Questa regola di formattazione condizionale evidenzia i valori unici nell'intervallo.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

