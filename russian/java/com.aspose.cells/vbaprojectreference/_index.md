---
title: "VbaProjectReference"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет ссылку проекта VBA."
type: docs
url: /ru/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

Представляет ссылку проекта VBA.

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
## Методы

| Метод | Описание |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | Получает расширенный Libid ссылки. |
| [getLibid()](#getLibid--) | Получает Libid ссылки. |
| [getName()](#getName--) | Получает имя ссылки. |
| [getRelativeLibid()](#getRelativeLibid--) | Получает идентификатор ссылочного проекта VBA с относительным путём. |
| [getTwiddledlibid()](#getTwiddledlibid--) | Получает twiddled Libid ссылки. |
| [getType()](#getType--) | Получает тип этой ссылки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | Устанавливает расширенный Libid ссылки. |
| [setLibid(String value)](#setLibid-java.lang.String-) | Устанавливает Libid ссылки. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя ссылки. |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | Устанавливает идентификатор ссылочного проекта VBA с относительным путём. |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | Устанавливает twiddled Libid ссылки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

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


Получает расширенный Libid ссылки.

**Remarks**

Только для ссылки управления.

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


Получает Libid ссылки.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Получает имя ссылки.

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


Получает идентификатор ссылочного проекта VBA с относительным путём.

**Remarks**

Только для ссылки на проект.

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


Получает twiddled Libid ссылки.

**Remarks**

Только для ссылки управления.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Получает тип этой ссылки.

Смотрите [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype).

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


Устанавливает расширенный Libid ссылки.

**Remarks**

Только для ссылки управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


Устанавливает Libid ссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя ссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


Устанавливает идентификатор ссылочного проекта VBA с относительным путём.

**Remarks**

Только для ссылки на проект.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


Устанавливает twiddled Libid ссылки.

**Remarks**

Только для ссылки управления.

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

