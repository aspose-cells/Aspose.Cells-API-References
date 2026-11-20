---
title: "LookInType"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il tipo di visualizzazione 'look in'."
type: docs
url: /it/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

Rappresenta il tipo di visualizzazione 'look in'.
## Campi

| Campo | Descrizione |
| --- | --- |
| [COMMENTS](#COMMENTS) | Trova l'oggetto solo dal commento della cella. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Trova l'oggetto solo dal valore formattato della cella([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [FORMULAS](#FORMULAS) | Trova l'oggetto cercato dalla formula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) se la cella è una formula, altrimenti lo trova dal valore originale della cella (stesso di [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)). |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Ignora le celle che non sono formule. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Trova l'oggetto solo dal valore originale della cella. |
| [VALUES](#VALUES) | Trova l'oggetto dal valore originale della cella([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) e dal valore formattato([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)). |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Ignora le celle che sono formule. |
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
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


Trova l'oggetto solo dal commento della cella. Ignora le celle che non hanno commenti.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


Trova l'oggetto solo dal valore formattato della cella([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


Trova l'oggetto cercato dalla formula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) se la cella è una formula, altrimenti lo trova dal valore originale della cella (stesso di [ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES)).

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


Ignora le celle che non sono formule. Per le celle che sono formule, trova l'oggetto ricercato dalla formula([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)).

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


Trova l'oggetto solo dal valore originale della cella.

### VALUES {#VALUES}
```
public static final int VALUES
```


Trova l'oggetto dal valore originale della cella([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) e dal valore formattato([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)).

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


Ignora le celle che sono formule. Per le celle che non sono formule, è lo stesso di [VALUES](../../com.aspose.cells/lookintype\#VALUES).

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

