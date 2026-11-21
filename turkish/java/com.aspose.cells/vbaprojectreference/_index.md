---
title: "VbaProjectReference"
second_title: "Aspose.Cells for Java API Referansı"
description: "VBA projesinin referansını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

VBA projesinin referansını temsil eder.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Referansın genişletilmiş Libid değerini al. |
| [getLibid()](#getLibid--) | Referansın Libid değerini al. |
| [getName()](#getName--) | Referansın adını al. |
| [getRelativeLibid()](#getRelativeLibid--) | Referans verilen VBA projesinin kimliğini göreceli bir yol ile al. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Referansın değiştirilen Libid değerini al. |
| [getType()](#getType--) | Bu referansın tipini al. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Referansın genişletilmiş Libid değerini ayarla. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Referansın Libid değerini ayarla. |
| [setName(String value)](#setName-java.lang.String-) | Referansın adını ayarla. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Referans verilen VBA projesinin kimliğini göreceli bir yol ile ayarla. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Referansın değiştirilen Libid değerini ayarla. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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


Referansın genişletilmiş Libid değerini al.

**Remarks**

Yalnızca kontrol referansı için.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Referansın Libid değerini al.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Referansın adını al.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Referans verilen VBA projesinin kimliğini göreceli bir yol ile al.

**Remarks**

Yalnızca proje referansı için.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Referansın değiştirilen Libid değerini al.

**Remarks**

Yalnızca kontrol referansı için.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Bu referansın tipini al.

Bakın [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

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


Referansın genişletilmiş Libid değerini ayarla.

**Remarks**

Yalnızca kontrol referansı için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Referansın Libid değerini ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Referansın adını ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Referans verilen VBA projesinin kimliğini göreceli bir yol ile ayarla.

**Remarks**

Yalnızca proje referansı için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Referansın değiştirilen Libid değerini ayarla.

**Remarks**

Yalnızca kontrol referansı için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

