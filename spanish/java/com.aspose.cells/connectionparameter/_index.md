---
title: "ConnectionParameter"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica propiedades sobre cualquier parámetro utilizado con conexiones de datos externas. Los parámetros son válidos para consultas ODBC y web."
type: docs
url: /es/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Especifica propiedades sobre cualquier parámetro utilizado con conexiones de datos externas. Los parámetros son válidos para consultas ODBC y web.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Referencia de celda que indica el valor de la celda a usar para el parámetro de consulta. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | El nombre del parámetro. |
| [getPrompt()](#getPrompt--) | Cadena de solicitud para el parámetro. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de una celda que proporciona el valor del parámetro cambia. |
| [getSqlType()](#getSqlType--) | Tipo de datos SQL del parámetro. |
| [getType()](#getType--) | Tipo de parámetro utilizado. |
| [getValue()](#getValue--) | Valor numérico no entero,valor entero,valor de cadena o valor booleano para usar como parámetro de consulta. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | Referencia de celda que indica el valor de la celda a usar para el parámetro de consulta. |
| [setName(String value)](#setName-java.lang.String-) | El nombre del parámetro. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | Cadena de solicitud para el parámetro. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de una celda que proporciona el valor del parámetro cambia. |
| [setSqlType(int value)](#setSqlType-int-) | Tipo de datos SQL del parámetro. |
| [setType(int value)](#setType-int-) | Tipo de parámetro utilizado. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Valor numérico no entero,valor entero,valor de cadena o valor booleano para usar como parámetro de consulta. |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Referencia de celda que indica el valor de la celda a usar para el parámetro de consulta. Se usa solo cuando parameterType es cell.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


El nombre del parámetro.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Cadena de solicitud para el parámetro. Presentada al usuario de la hoja de cálculo junto con la interfaz de entrada para recopilar el valor del parámetro antes de actualizar los datos externos. Se usa solo cuando parameterType = prompt.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de una celda que proporciona el valor del parámetro cambia. Si es verdadero, los datos externos se actualizan usando el nuevo valor del parámetro cada vez que hay un cambio. Si es falso, los datos externos solo se actualizan cuando el usuario lo solicita, o cuando otro evento desencadena la actualización (p. ej., al abrir el libro).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


Tipo de datos SQL del parámetro. Solo válido para fuentes ODBC.

Ver [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Tipo de parámetro utilizado. Si parameterType=valor, entonces se usará el valor de boolean, double, integer o string. En este caso, se espera que solo se especifique uno de \{boolean, double, integer, or string\}.

Ver [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Valor numérico no entero,valor entero,valor de cadena o valor Booleano para usar como parámetro de consulta. Se usa solo cuando parameterType es value.

**Returns:**
java.lang.Object
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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


Referencia de celda que indica el valor de la celda a usar para el parámetro de consulta. Se usa solo cuando parameterType es cell.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


El nombre del parámetro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


Cadena de solicitud para el parámetro. Presentada al usuario de la hoja de cálculo junto con la interfaz de entrada para recopilar el valor del parámetro antes de actualizar los datos externos. Se usa solo cuando parameterType = prompt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de una celda que proporciona el valor del parámetro cambia. Si es verdadero, los datos externos se actualizan usando el nuevo valor del parámetro cada vez que hay un cambio. Si es falso, los datos externos solo se actualizan cuando el usuario lo solicita, o cuando otro evento desencadena la actualización (p. ej., al abrir el libro).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


Tipo de datos SQL del parámetro. Solo válido para fuentes ODBC.

Ver [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Tipo de parámetro utilizado. Si parameterType=valor, entonces se usará el valor de boolean, double, integer o string. En este caso, se espera que solo se especifique uno de \{boolean, double, integer, or string\}.

Ver [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Valor numérico no entero,valor entero,valor de cadena o valor Booleano para usar como parámetro de consulta. Se usa solo cuando parameterType es value.

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

