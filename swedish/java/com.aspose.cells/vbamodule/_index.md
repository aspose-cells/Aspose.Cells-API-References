---
title: "VbaModule"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar modulen i VBA-projektet."
type: docs
url: /sv/java/com.aspose.cells/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public class VbaModule
```

Representerar modulen i VBA-projektet.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBinaryCodes()](#getBinaryCodes--) | Hämtar modulens binära koder. |
| [getClass()](#getClass--) |  |
| [getCodes()](#getCodes--) | Hämtar modulens koder. |
| [getName()](#getName--) | Hämtar namnet på Module. |
| [getType()](#getType--) | Hämtar typen av modul. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCodes(String value)](#setCodes-java.lang.String-) | Ställer in koderna för modul. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på Module. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBinaryCodes() {#getBinaryCodes--}
```
public byte[] getBinaryCodes()
```


Hämtar modulens binära koder.

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


Hämtar modulens koder.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på Module.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av modul.

Se [VbaModuleType](../../com.aspose.cells/vbamoduletype).

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


Ställer in koderna för modul.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på Module.

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

