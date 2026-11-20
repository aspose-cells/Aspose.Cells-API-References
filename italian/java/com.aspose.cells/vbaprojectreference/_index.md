---
title: "VbaProjectReference"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il riferimento del progetto VBA."
type: docs
url: /it/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

Rappresenta il riferimento del progetto VBA.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Ottiene il Libid esteso del riferimento. |
| [getLibid()](#getLibid--) | Ottiene il Libid del riferimento. |
| [getName()](#getName--) | Ottiene il nome del riferimento. |
| [getRelativeLibid()](#getRelativeLibid--) | Ottiene l'identificatore del progetto VBA di riferimento con un percorso relativo. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Ottiene il Libid modificato del riferimento. |
| [getType()](#getType--) | Ottiene il tipo di questo riferimento. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Imposta il Libid esteso del riferimento. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Imposta il Libid del riferimento. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome del riferimento. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Imposta l'identificatore del progetto VBA di riferimento con un percorso relativo. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Imposta il Libid modificato del riferimento. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

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
### getExtendedLibid() {#getExtendedLibid--}
```
public String getExtendedLibid()
```


Ottiene il Libid esteso del riferimento.

**Remarks**

Solo per riferimento di controllo

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Ottiene il Libid del riferimento.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del riferimento.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Ottiene l'identificatore del progetto VBA di riferimento con un percorso relativo.

**Remarks**

Solo per riferimento del progetto.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Ottiene il Libid modificato del riferimento.

**Remarks**

Solo per riferimento di controllo

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di questo riferimento.

Vedi [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

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


Imposta il Libid esteso del riferimento.

**Remarks**

Solo per riferimento di controllo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Imposta il Libid del riferimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome del riferimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Imposta l'identificatore del progetto VBA di riferimento con un percorso relativo.

**Remarks**

Solo per riferimento del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Imposta il Libid modificato del riferimento.

**Remarks**

Solo per riferimento di controllo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

