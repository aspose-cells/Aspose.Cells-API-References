---
title: "VbaProjectReference"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مرجع مشروع VBA."
type: docs
url: /ar/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

يمثل مرجع مشروع VBA.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | يحصل على Libid الموسع للمرجع. |
| [getLibid()](#getLibid--) | يحصل على Libid للمرجع. |
| [getName()](#getName--) | يحصل على اسم المرجع. |
| [getRelativeLibid()](#getRelativeLibid--) | يحصل على معرّف مشروع VBA المرجعي بمسار نسبي. |
| [getTwiddledlibid()](#getTwiddledlibid--) | يحصل على Libid المعدل للمرجع. |
| [getType()](#getType--) | يحصل على نوع هذا المرجع. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | يضبط Libid الموسع للمرجع. |
| [setLibid(String value)](#setLibid-java.lang.String-) | يضبط Libid للمرجع. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم المرجع. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | يضبط معرّف مشروع VBA المرجعي بمسار نسبي. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | يضبط Libid المعدل للمرجع. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحصل على Libid الموسع للمرجع.

**Remarks**

فقط للمرجع التحكم.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


يحصل على Libid للمرجع.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم المرجع.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


يحصل على معرّف مشروع VBA المرجعي بمسار نسبي.

**Remarks**

فقط للمرجع المشروع.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


يحصل على Libid المعدل للمرجع.

**Remarks**

فقط للمرجع التحكم.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع هذا المرجع.

انظر [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

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


يضبط Libid الموسع للمرجع.

**Remarks**

فقط للمرجع التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


يضبط Libid للمرجع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم المرجع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


يضبط معرّف مشروع VBA المرجعي بمسار نسبي.

**Remarks**

فقط للمرجع المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


يضبط Libid المعدل للمرجع.

**Remarks**

فقط للمرجع التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

