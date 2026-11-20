---
title: "AbstractLowCodeProtectionProvider"
second_title: "Справочник API Aspose.Cells for Java"
description: "Реализация, предоставляющая настройки защиты"
type: docs
url: /ru/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

Реализация, предоставляющая настройки защиты
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Получает пароль для открытия файла таблицы. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Получает пароль для защиты книги с указанным типом защиты. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Получает тип защиты для защиты книги. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Получает пароль для защиты указанного листа. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Получает тип защиты для защиты указанного листа. |
| [getWritePassword()](#getWritePassword--) | Получает пароль для изменения файла таблицы. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
```


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
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


Получает пароль для открытия файла таблицы.

**Returns:**
java.lang.String - Пароль для открытия файла таблицы. Пустая строка означает отсутствие защиты при открытии файла.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


Получает пароль для защиты книги с указанным типом защиты.

**Returns:**
java.lang.String - Пароль для защиты книги.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


Получает тип защиты для защиты книги.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Тип защиты для защиты книги. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) означает отсутствие защиты для книги.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


Получает пароль для защиты указанного листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - Пароль для защиты указанного листа.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


Получает тип защиты для защиты указанного листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Тип защиты для защиты указанного листа. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) означает отсутствие защиты листа.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


Получает пароль для изменения файла таблицы.

**Returns:**
java.lang.String - Пароль для изменения файла электронной таблицы. Пустое значение означает отсутствие защиты для изменения файла.
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

