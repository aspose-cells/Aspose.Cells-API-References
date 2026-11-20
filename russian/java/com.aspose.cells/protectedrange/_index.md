---
title: "ProtectedRange"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указанный диапазон, разрешённый для редактирования, когда защита листа включена."
type: docs
url: /ru/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

Указанный диапазон, разрешённый для редактирования, когда защита листа включена.
## Методы

| Метод | Описание |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Добавляет ссылочную область к этому |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Получает все ссылочные области. |
| [getCellArea()](#getCellArea--) | Получает объект [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) , представляющий область ячейки, которую нужно защитить. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Получает название диапазона. |
| [getPassword()](#getPassword--) | Представляет пароль для защиты диапазона. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | Дескриптор безопасности определяет учетные записи пользователей, которые могут редактировать этот диапазон без предоставления пароля для доступа к диапазону. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Указывает, защищен ли лист паролем. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Получает название диапазона. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Представляет пароль для защиты диапазона. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | Дескриптор безопасности определяет учетные записи пользователей, которые могут редактировать этот диапазон без предоставления пароля для доступа к диапазону. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


Добавляет ссылочную область к этому

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | int | Начальная строка. |
| startColumn | int | Начальный столбец. |
| endRow | int | Конечная строка. |
| endColumn | int | Конечный столбец. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Получает все ссылочные области.

**Returns:**
com.aspose.cells.CellArea[] - Возвращает все ссылочные области.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Получает объект [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) , представляющий область ячейки, которую нужно защитить.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Получает название диапазона. Это используется как дескриптор, а не как определение именованного диапазона.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


Представляет пароль для защиты диапазона.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


Дескриптор безопасности определяет учетные записи пользователей, которые могут редактировать этот диапазон без предоставления пароля для доступа к диапазону.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Указывает, защищен ли лист паролем.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Получает название диапазона. Это используется как дескриптор, а не как определение именованного диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Представляет пароль для защиты диапазона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


Дескриптор безопасности определяет учетные записи пользователей, которые могут редактировать этот диапазон без предоставления пароля для доступа к диапазону.

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

