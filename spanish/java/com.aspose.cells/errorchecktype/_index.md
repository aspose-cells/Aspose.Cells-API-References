---
title: "ErrorCheckType"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todos los tipos de comprobación de errores."
type: docs
url: /es/java/com.aspose.cells/errorchecktype/
---

**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```

Representa todos los tipos de comprobación de errores.
## Campos

| Campo | Descripción |
| --- | --- |
| [CALC](#CALC) | **Observaciones** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | Ignorar errores cuando las celdas contienen un valor diferente de la fórmula calculada de la columna. |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | Ignorar errores cuando las fórmulas hacen referencia a celdas vacías. |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | Ignorar errores cuando las celdas contienen fórmulas que generan un error. |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | Ignorar errores cuando una fórmula en una región de su hoja de cálculo difiere de otras fórmulas en la misma región. |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | Ignorar errores cuando las fórmulas omiten ciertas celdas en una región. |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | Ignorar errores cuando los números están formateados como texto o van precedidos de una comilla simple. |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | Ignorar errores cuando el valor de una celda en una Tabla no cumple con las reglas de Validación de datos especificadas. |
| [TEXT_DATE](#TEXT-DATE) | Ignorar errores cuando las fórmulas contienen celdas con formato de texto donde los años se representan con 2 dígitos. |
| [TEXT_NUMBER](#TEXT-NUMBER) | Ignorar errores cuando los números están formateados como texto o van precedidos de una comilla simple. |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | Ignorar errores cuando las fórmulas contienen celdas con formato de texto donde los años se representan con 2 dígitos. |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | Ignorar errores cuando las celdas desbloqueadas contienen fórmulas. |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | Ignorar errores cuando las celdas desbloqueadas contienen fórmulas. |
| [VALIDATION](#VALIDATION) | Ignorar errores cuando el valor de una celda en una Tabla no cumple con las reglas de Validación de datos especificadas. |
## Métodos

| Método | Descripción |
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

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el enum ErrorCheckType.EvaluationError. Este método será eliminado 12 meses después desde octubre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```


Ignorar errores cuando las celdas contienen un valor diferente de la fórmula calculada de la columna.

### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```


Ignorar errores cuando las fórmulas hacen referencia a celdas vacías.

### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```


Ignorar errores cuando las celdas contienen fórmulas que generan un error.

### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```


Ignorar errores cuando una fórmula en una región de su hoja de cálculo difiere de otras fórmulas en la misma región.

### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```


Ignorar errores cuando las fórmulas omiten ciertas celdas en una región.

### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```


Ignorar errores cuando los números están formateados como texto o van precedidos de una comilla simple.

### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```


Ignorar errores cuando el valor de una celda en una Tabla no cumple con las reglas de Validación de datos especificadas.

### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```


Ignorar errores cuando las fórmulas contienen celdas con formato de texto donde los años se representan con 2 dígitos.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el enum ErrorCheckType.TwoDigitTextYear. Este método será eliminado 12 meses después desde octubre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```


Ignorar errores cuando los números están formateados como texto o van precedidos de una comilla simple.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el enum ErrorCheckType.NumberStoredAsText. Este método será eliminado 12 meses después desde octubre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```


Ignorar errores cuando las fórmulas contienen celdas con formato de texto donde los años se representan con 2 dígitos.

### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```


Ignorar errores cuando las celdas desbloqueadas contienen fórmulas.

### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```


Ignorar errores cuando las celdas desbloqueadas contienen fórmulas.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el enum ErrorCheckType.UnproctedFormula. Este método será eliminado 12 meses después desde octubre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Ignorar errores cuando el valor de una celda en una Tabla no cumple con las reglas de Validación de datos especificadas.

**Remarks**

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el enum ErrorCheckType.TableDataValidation. Este método será eliminado 12 meses después desde octubre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

