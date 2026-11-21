---
title: "ReferredArea"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un área referida por la fórmula."
type: docs
url: /es/java/com.aspose.cells/referredarea/
---

**Inheritance:**
java.lang.Object
```
public class ReferredArea
```

Representa un área referida por la fórmula.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | La columna final del área. |
| [getEndRow()](#getEndRow--) | La fila final del área. |
| [getExternalFileName()](#getExternalFileName--) | Obtén el nombre del archivo externo si esto es una referencia externa. |
| [getSheetName()](#getSheetName--) | Indica en qué hoja se encuentra esta referencia. |
| [getSheetNames()](#getSheetNames--) | Nombres de todas las hojas de cálculo a las que esta instancia hace referencia. |
| [getStartColumn()](#getStartColumn--) | La columna inicial del área. |
| [getStartRow()](#getStartRow--) | La fila inicial del área. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área. |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área. |
| [getValues()](#getValues--) | Obtiene los valores de las celdas en esta área. |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | Obtiene los valores de las celdas en esta área. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Indica si esto es un área. |
| [isEntireColumn()](#isEntireColumn--) | Indica si esta área contiene todas las filas (columna completa). |
| [isEntireRow()](#isEntireRow--) | Indica si esta área contiene todas las columnas (fila completa). |
| [isExternalLink()](#isExternalLink--) | Indica si esto es un enlace externo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Devuelve la dirección de referencia de esta área. |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


La columna final del área.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


La fila final del área.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


Obtén el nombre del archivo externo si esto es una referencia externa.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Indica en qué hoja se encuentra esta referencia.

**Remarks**

Si hace referencia a varias hojas de cálculo, el valor devuelto es como la expresión de rango en la fórmula. Por ejemplo \"Sheet1:Sheet3\" para la referencia en la fórmula \"=SUM(Sheet1:Sheet3!$A$1:$B$2)\".

**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```


Nombres de todas las hojas de cálculo a las que esta instancia hace referencia.

**Returns:**
java.lang.String[]
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


La columna inicial del área.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


La fila inicial del área.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | desplazamiento de fila desde la fila inicial de esta área |
| colOffset | int | desplazamiento de columna desde la fila inicial de esta área |

**Returns:**
java.lang.Object - \"\\#REF!\" si esta área es inválida; \"\\#N/A\" si el desplazamiento dado está fuera de esta área; de lo contrario devuelve el valor de la celda en la posición indicada.
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```


Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | int | desplazamiento de fila desde la fila inicial de esta área |
| colOffset | int | desplazamiento de columna desde la fila inicial de esta área |
| calculateFormulas | boolean | Si se debe calcular recursivamente cuando la referencia especificada es una fórmula |

**Returns:**
java.lang.Object - \"\\#REF!\" si esta área es inválida; \"\\#N/A\" si el desplazamiento dado está fuera de esta área; de lo contrario devuelve el valor de la celda en la posición indicada.
### getValues() {#getValues--}
```
public Object getValues()
```


Obtiene los valores de las celdas en esta área.

**Returns:**
java.lang.Object - Si esta área es inválida, se devolverá \"\\#REF!\"; si esta área es una sola celda, se devolverá el objeto valor de la celda; de lo contrario se devuelve una matriz 2D con todos los valores de esta área.
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```


Obtiene los valores de las celdas en esta área.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calculateFormulas | boolean | En este rango, si hay algunas fórmulas que no se han calculado, esta bandera indica si esas fórmulas deben calcularse recursivamente |

**Returns:**
java.lang.Object - Si esta área es inválida, se devolverá \"\\#REF!\"; si esta área es una sola celda, se devolverá el objeto valor de la celda; de lo contrario se devuelve una matriz 2D con todos los valores de esta área.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Indica si esto es un área.

**Remarks**

Si esto no es un área, solo afectan StartRow y StartColumn.

**Returns:**
boolean
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```


Indica si esta área contiene todas las filas (columna completa).

**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```


Indica si esta área contiene todas las columnas (fila completa).

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Indica si esto es un enlace externo.

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




### toString() {#toString--}
```
public String toString()
```


Devuelve la dirección de referencia de esta área. Generalmente es la dirección de la referencia que puede usarse en una fórmula, como \"Sheet1!A1:C3\".

**Returns:**
java.lang.String - la dirección de referencia de esta área.
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

