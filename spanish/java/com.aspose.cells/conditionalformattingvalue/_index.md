---
title: "ConditionalFormattingValue"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Describe los valores de los puntos de interpolación en una barra de datos de escala degradada o conjunto de iconos."
type: docs
url: /es/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Describe los valores de los puntos de interpolación en una escala de degradado, dataBar o iconSet.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Obtiene el tipo de este objeto de valor de formato condicional. |
| [getValue()](#getValue--) | Obtiene el valor de este objeto de valor de formato condicional. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Obtiene la bandera Mayor o Igual. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Establece la bandera Mayor o Igual. |
| [setType(int value)](#setType-int-) | Establece el tipo de este objeto de valor de formato condicional. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Establece el valor de este objeto de valor de formato condicional. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de este objeto de valor de formato condicional. Establecer el tipo a FormatConditionValueType.Min o FormatConditionValueType.Max establecerá automáticamente "Value" a null.

Ver [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor de este objeto de valor de formato condicional. Debe usarse junto con Type.

**Remarks**

Si el valor es una cadena y comienza con "=", se procesará como una fórmula; de lo contrario lo procesaremos como un valor simple.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


Obtiene la bandera Mayor o Igual. Úsese solo para conjuntos de iconos, determina si este valor de umbral usa el operador mayor o igual que. 'false' indica que se usa 'mayor que' en lugar de 'mayor o igual que'. El valor predeterminado es true.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


Establece la bandera Mayor o Igual. Úsese solo para conjuntos de iconos, determina si este valor de umbral usa el operador mayor o igual que. 'false' indica que se usa 'mayor que' en lugar de 'mayor o igual que'. El valor predeterminado es true.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Establece el tipo de este objeto de valor de formato condicional. Establecer el tipo a FormatConditionValueType.Min o FormatConditionValueType.Max establecerá automáticamente "Value" a null.

Ver [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Establece el valor de este objeto de valor de formato condicional. Debe usarse junto con Type.

**Remarks**

Si el valor es una cadena y comienza con "=", se procesará como una fórmula; de lo contrario lo procesaremos como un valor simple.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

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

