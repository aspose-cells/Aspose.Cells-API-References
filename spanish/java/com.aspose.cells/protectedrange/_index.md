---
title: "ProtectedRange"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Un rango especificado que se permite editar cuando la protección de la hoja está ACTIVADA."
type: docs
url: /es/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

Un rango especificado que se permite editar cuando la protección de la hoja está ACTIVADA.
## Métodos

| Método | Descripción |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Agrega un área referenciada a este |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Obtiene todas las áreas referenciadas. |
| [getCellArea()](#getCellArea--) | Obtiene el [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) objeto que representa el área de celda a proteger. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Obtiene el título del rango. |
| [getPassword()](#getPassword--) | Representa la contraseña para proteger el rango. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indica si la hoja de cálculo está protegida con contraseña. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Obtiene el título del rango. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Representa la contraseña para proteger el rango. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


Agrega un área referenciada a este

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | int | La fila inicial. |
| startColumn | int | La columna inicial. |
| endRow | int | La fila final. |
| endColumn | int | La columna final. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Obtiene todas las áreas referenciadas.

**Returns:**
com.aspose.cells.CellArea[] - Devuelve todas las áreas referenciadas.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Obtiene el [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) objeto que representa el área de celda a proteger.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
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


Obtiene el título del rango. Esto se usa como descriptor, no como una definición de rango nombrado.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


Representa la contraseña para proteger el rango.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Indica si la hoja de cálculo está protegida con contraseña.

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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Obtiene el título del rango. Esto se usa como descriptor, no como una definición de rango nombrado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Representa la contraseña para proteger el rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

