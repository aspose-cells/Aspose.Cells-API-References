---
title: "ExternalLink"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un enlace externo en un libro de trabajo."
type: docs
url: /es/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

Representa un enlace externo en un libro de trabajo.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Agrega un nombre externo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Representa la fuente de datos del enlace externo. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Representa la fuente de datos almacenada del enlace externo. |
| [getPathType()](#getPathType--) | Obtén el tipo de ruta de este enlace externo |
| [getType()](#getType--) | Obtiene el tipo de enlace externo. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indica si este enlace externo es referenciado por otros. |
| [isVisible()](#isVisible--) | Indica si este enlace externo es visible en MS Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Representa la fuente de datos del enlace externo. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Representa la fuente de datos almacenada del enlace externo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


Agrega un nombre externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | java.lang.String | El texto del nombre externo. Si el nombre externo pertenece a una hoja de cálculo, el texto debe ser como Sheet1!Text. |
| referTo | java.lang.String | El referTo del nombre externo. Debe ser una celda o el rango. |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


Representa la fuente de datos del enlace externo.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


Representa la fuente de datos almacenada del enlace externo.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


Obtén el tipo de ruta de este enlace externo

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de enlace externo.

Ver [ExternalLinkType](../../com.aspose.cells/externallinktype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Indica si este enlace externo es referenciado por otros.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica si este enlace externo es visible en MS Excel.

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




### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```


Representa la fuente de datos del enlace externo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


Representa la fuente de datos almacenada del enlace externo.

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

