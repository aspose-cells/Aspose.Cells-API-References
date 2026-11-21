---
title: "VbaProjectReference"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar referensen till VBA-projektet."
type: docs
url: /sv/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

Representerar referensen till VBA-projektet.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Hämtar det utökade Libid för referensen. |
| [getLibid()](#getLibid--) | Hämtar Libid för referensen. |
| [getName()](#getName--) | Hämtar namnet på referensen. |
| [getRelativeLibid()](#getRelativeLibid--) | Hämtar identifieraren för det refererade VBA-projektet med en relativ sökväg. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Hämtar det manipulerade Libid för referensen. |
| [getType()](#getType--) | Hämtar typen av denna referens. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Anger det utökade Libid för referensen. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Anger Libid för referensen. |
| [setName(String value)](#setName-java.lang.String-) | Anger namnet på referensen. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Anger identifieraren för det refererade VBA-projektet med en relativ sökväg. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Anger det manipulerade Libid för referensen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Hämtar det utökade Libid för referensen.

**Remarks**

Endast för kontrollreferens.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Hämtar Libid för referensen.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på referensen.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Hämtar identifieraren för det refererade VBA-projektet med en relativ sökväg.

**Remarks**

Endast för projektreferens.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Hämtar det manipulerade Libid för referensen.

**Remarks**

Endast för kontrollreferens.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av denna referens.

Se [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

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


Anger det utökade Libid för referensen.

**Remarks**

Endast för kontrollreferens.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Anger Libid för referensen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Anger namnet på referensen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Anger identifieraren för det refererade VBA-projektet med en relativ sökväg.

**Remarks**

Endast för projektreferens.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Anger det manipulerade Libid för referensen.

**Remarks**

Endast för kontrollreferens.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

