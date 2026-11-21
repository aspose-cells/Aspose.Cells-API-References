---
title: "VbaModule"
second_title: "Aspose.Cells for Java API Referansı"
description: "VBA projesindeki modülü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public class VbaModule
```

VBA projesindeki modülü temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         int index = vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         // Get vba module
         VbaModule vbaModule = vbaProject.getModules().get(index);
         // Set codes
         vbaModule.setCodes("Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBinaryCodes()](#getBinaryCodes--) | Modülün ikili kodlarını alır. |
| [getClass()](#getClass--) |  |
| [getCodes()](#getCodes--) | Modülün kodlarını alır. |
| [getName()](#getName--) | Modülün adını alır. |
| [getType()](#getType--) | Modülün türünü alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCodes(String value)](#setCodes-java.lang.String-) | Modülün kodlarını ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Modülün adını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBinaryCodes() {#getBinaryCodes--}
```
public byte[] getBinaryCodes()
```


Modülün ikili kodlarını alır.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodes() {#getCodes--}
```
public String getCodes()
```


Modülün kodlarını alır.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Modülün adını alır.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Modülün türünü alır.

Bakınız [VbaModuleType](../../com.aspose.cells/vbamoduletype).

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




### setCodes(String value) {#setCodes-java.lang.String-}
```
public void setCodes(String value)
```


Modülün kodlarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Modülün adını ayarlar.

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

