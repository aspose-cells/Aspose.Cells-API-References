---
title: "VbaProjectReference"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Referenz des VBA‑Projekts dar."
type: docs
url: /de/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

Stellt die Referenz des VBA‑Projekts dar.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Ermittelt die erweiterte Libid der Referenz. |
| [getLibid()](#getLibid--) | Ermittelt die Libid der Referenz. |
| [getName()](#getName--) | Ermittelt den Namen der Referenz. |
| [getRelativeLibid()](#getRelativeLibid--) | Ermittelt den Bezeichner des referenzierten VBA-Projekts mit einem relativen Pfad. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Ermittelt die twiddled Libid der Referenz. |
| [getType()](#getType--) | Ermittelt den Typ dieser Referenz. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Legt die erweiterte Libid der Referenz fest. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Legt die Libid der Referenz fest. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen der Referenz fest. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Legt den Bezeichner des referenzierten VBA-Projekts mit einem relativen Pfad fest. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Legt die manipulierte Libid der Referenz fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Ermittelt die erweiterte Libid der Referenz.

**Remarks**

Nur für Steuerungsreferenz.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Ermittelt die Libid der Referenz.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Ermittelt den Namen der Referenz.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Ermittelt den Bezeichner des referenzierten VBA-Projekts mit einem relativen Pfad.

**Remarks**

Nur für Projektreferenz.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Ermittelt die twiddled Libid der Referenz.

**Remarks**

Nur für Steuerungsreferenz.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Ermittelt den Typ dieser Referenz.

Siehe [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

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


Legt die erweiterte Libid der Referenz fest.

**Remarks**

Nur für Steuerungsreferenz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Legt die Libid der Referenz fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Legt den Namen der Referenz fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Legt den Bezeichner des referenzierten VBA-Projekts mit einem relativen Pfad fest.

**Remarks**

Nur für Projektreferenz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Legt die manipulierte Libid der Referenz fest.

**Remarks**

Nur für Steuerungsreferenz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

