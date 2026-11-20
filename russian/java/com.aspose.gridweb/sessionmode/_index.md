---
title: "SessionMode"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет режим сеанса сетки."
type: docs
url: /ru/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

Представляет режим сеанса сетки.
## Поля

| Поле | Описание |
| --- | --- |
| [CUSTOM](#CUSTOM) | Использует событие LoadCustomData для ручной загрузки данных листа сетки автоматически. |
| [FILE](#FILE) | Использует системный файл для автоматического сохранения/восстановления данных листа сетки, пользователь должен установить SessionStorePath для указания каталога файлов. |
| [SESSION](#SESSION) | Использует системную сессию для автоматического сохранения/восстановления данных листа сетки. |
| [VIEW_STATE](#VIEW-STATE) | Использует viewstate страницы для автоматического сохранения/восстановления данных листа сетки. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Использует событие LoadCustomData для ручной загрузки данных листа сетки. И использует событие SheetDataUpdated для сохранения данных листа сетки.

### FILE {#FILE}
```
public static final int FILE
```


Использует системный файл для автоматического сохранения/восстановления данных листа сетки, пользователь должен установить SessionStorePath для указания каталога файлов.

### SESSION {#SESSION}
```
public static final int SESSION
```


Использует системную сессию для автоматического сохранения/восстановления данных листа сетки.

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


Использует viewstate страницы для автоматического сохранения/восстановления данных листа сетки.

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

