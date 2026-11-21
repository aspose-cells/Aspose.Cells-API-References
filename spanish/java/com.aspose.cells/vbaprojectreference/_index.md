---
title: "VbaProjectReference"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la referencia del proyecto VBA."
type: docs
url: /es/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

Representa la referencia del proyecto VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Obtiene el Libid extendido de la referencia. |
| [getLibid()](#getLibid--) | Obtiene el Libid de la referencia. |
| [getName()](#getName--) | Obtiene el nombre de la referencia. |
| [getRelativeLibid()](#getRelativeLibid--) | Obtiene el identificador del proyecto VBA referenciado con una ruta relativa. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Obtiene el Libid retorcido de la referencia. |
| [getType()](#getType--) | Obtiene el tipo de esta referencia. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Establece el Libid extendido de la referencia. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Establece el Libid de la referencia. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la referencia. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Establece el identificador del proyecto VBA referenciado con una ruta relativa. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Establece el Libid retorcido de la referencia. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

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
### getExtendedLibid() {#getExtendedLibid--}
```
public String getExtendedLibid()
```


Obtiene el Libid extendido de la referencia.

**Remarks**

Solo para referencia de control.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Obtiene el Libid de la referencia.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la referencia.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Obtiene el identificador del proyecto VBA referenciado con una ruta relativa.

**Remarks**

Solo para referencia del proyecto.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Obtiene el Libid retorcido de la referencia.

**Remarks**

Solo para referencia de control.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de esta referencia.

Ver [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

**Returns:**
int
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




### setExtendedLibid(String value) {#setExtendedLibid-java.lang.String-}
```
public void setExtendedLibid(String value)
```


Establece el Libid extendido de la referencia.

**Remarks**

Solo para referencia de control.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Establece el Libid de la referencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Establece el nombre de la referencia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Establece el identificador del proyecto VBA referenciado con una ruta relativa.

**Remarks**

Solo para referencia del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Establece el Libid retorcido de la referencia.

**Remarks**

Solo para referencia de control.

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

