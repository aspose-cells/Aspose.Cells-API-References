---
title: "VbaModule"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет модуль в проекте VBA."
type: docs
url: /ru/java/com.aspose.cells/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public class VbaModule
```

Представляет модуль в проекте VBA.

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
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBinaryCodes()](#getBinaryCodes--) | Получает бинарные коды модуля. |
| [getClass()](#getClass--) |  |
| [getCodes()](#getCodes--) | Получает коды модуля. |
| [getName()](#getName--) | Получает имя модуля. |
| [getType()](#getType--) | Получает тип модуля. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCodes(String value)](#setCodes-java.lang.String-) | Устанавливает коды модуля. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя модуля. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBinaryCodes() {#getBinaryCodes--}
```
public byte[] getBinaryCodes()
```


Получает бинарные коды модуля.

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


Получает коды модуля.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Получает имя модуля.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Получает тип модуля.

Смотрите [VbaModuleType](../../com.aspose.cells/vbamoduletype).

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


Устанавливает коды модуля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя модуля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

