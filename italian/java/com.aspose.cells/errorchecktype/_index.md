---
title: "ErrorCheckType"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutti i tipi di verifica errori."
type: docs
url: /it/java/com.aspose.cells/errorchecktype/
---

**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```

Rappresenta tutti i tipi di verifica errori.
## Campi

| Campo | Descrizione |
| --- | --- |
| [CALC](#CALC) | **Osservazioni** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | Ignora gli errori quando le celle contengono un valore diverso dalla formula calcolata della colonna. |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | Ignora gli errori quando le formule fanno riferimento a celle vuote. |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | Ignora gli errori quando le celle contengono formule che generano un errore. |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | Ignora gli errori quando una formula in un'area del foglio di lavoro differisce dalle altre formule nella stessa area. |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | Ignora gli errori quando le formule omettono alcune celle in un'area. |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | Ignora gli errori quando i numeri sono formattati come testo o sono preceduti da un apostrofo |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | Ignora gli errori quando il valore di una cella in una tabella non rispetta le regole di convalida dei dati specificate. |
| [TEXT_DATE](#TEXT-DATE) | Ignora gli errori quando le formule contengono celle formattate come testo con anni rappresentati con 2 cifre. |
| [TEXT_NUMBER](#TEXT-NUMBER) | Ignora gli errori quando i numeri sono formattati come testo o sono preceduti da un apostrofo |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | Ignora gli errori quando le formule contengono celle formattate come testo con anni rappresentati con 2 cifre. |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | Ignora gli errori quando le celle sbloccate contengono formule. |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | Ignora gli errori quando le celle sbloccate contengono formule. |
| [VALIDATION](#VALIDATION) | Ignora gli errori quando il valore di una cella in una tabella non rispetta le regole di convalida dei dati specificate. |
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
### CALC {#CALC}
```
public static final int CALC
```


**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare l'enumerazione ErrorCheckType.EvaluationError. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```


Ignora gli errori quando le celle contengono un valore diverso dalla formula calcolata della colonna.

### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```


Ignora gli errori quando le formule fanno riferimento a celle vuote.

### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```


Ignora gli errori quando le celle contengono formule che generano un errore.

### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```


Ignora gli errori quando una formula in un'area del foglio di lavoro differisce dalle altre formule nella stessa area.

### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```


Ignora gli errori quando le formule omettono alcune celle in un'area.

### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```


Ignora gli errori quando i numeri sono formattati come testo o sono preceduti da un apostrofo

### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```


Ignora gli errori quando il valore di una cella in una tabella non rispetta le regole di convalida dei dati specificate.

### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```


Ignora gli errori quando le formule contengono celle formattate come testo con anni rappresentati con 2 cifre.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare l'enumerazione ErrorCheckType.TwoDigitTextYear. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```


Ignora gli errori quando i numeri sono formattati come testo o sono preceduti da un apostrofo

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare l'enumerazione ErrorCheckType.NumberStoredAsText. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```


Ignora gli errori quando le formule contengono celle formattate come testo con anni rappresentati con 2 cifre.

### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```


Ignora gli errori quando le celle sbloccate contengono formule.

### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```


Ignora gli errori quando le celle sbloccate contengono formule.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare l'enumerazione ErrorCheckType.UnproctedFormula. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Ignora gli errori quando il valore di una cella in una tabella non rispetta le regole di convalida dei dati specificate.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare l'enumerazione ErrorCheckType.TableDataValidation. Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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

