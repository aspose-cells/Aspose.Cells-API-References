---
title: VbaProjectReference
second_title: Aspose.Cells for Java API Reference
description: Represents the reference of VBA project.
type: docs
weight: 629
url: /java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

Represents the reference of VBA project.

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
## Methods

| Method | Description |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Gets and sets the extended Libid of the reference. |
| [getLibid()](#getLibid--) | Gets and sets the Libid of the reference. |
| [getName()](#getName--) | Gets and sets the name of the reference. |
| [getRelativeLibid()](#getRelativeLibid--) | Gets and sets the referenced VBA project's identifier with an relative path. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Gets and sets the twiddled Libid of the reference. |
| [getType()](#getType--) | Gets the type of this reference. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Please see the getter of this property: [getExtendedLibid()](../../com.aspose.cells/vbaprojectreference\#getExtendedLibid--) |
| [setLibid(String value)](#setLibid-java.lang.String-) | Please see the getter of this property: [getLibid()](../../com.aspose.cells/vbaprojectreference\#getLibid--) |
| [setName(String value)](#setName-java.lang.String-) | Please see the getter of this property: [getName()](../../com.aspose.cells/vbaprojectreference\#getName--) |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Please see the getter of this property: [getRelativeLibid()](../../com.aspose.cells/vbaprojectreference\#getRelativeLibid--) |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Please see the getter of this property: [getTwiddledlibid()](../../com.aspose.cells/vbaprojectreference\#getTwiddledlibid--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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


Gets and sets the extended Libid of the reference. Only for control reference.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Gets and sets the Libid of the reference.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Gets and sets the name of the reference.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Gets and sets the referenced VBA project's identifier with an relative path. Only for project reference.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Gets and sets the twiddled Libid of the reference. Only for control reference.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Gets the type of this reference.

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


Please see the getter of this property: [getExtendedLibid()](../../com.aspose.cells/vbaprojectreference\#getExtendedLibid--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Please see the getter of this property: [getLibid()](../../com.aspose.cells/vbaprojectreference\#getLibid--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Please see the getter of this property: [getName()](../../com.aspose.cells/vbaprojectreference\#getName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Please see the getter of this property: [getRelativeLibid()](../../com.aspose.cells/vbaprojectreference\#getRelativeLibid--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Please see the getter of this property: [getTwiddledlibid()](../../com.aspose.cells/vbaprojectreference\#getTwiddledlibid--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

