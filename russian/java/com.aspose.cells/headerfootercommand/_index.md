---
title: "HeaderFooterCommand"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет команду заголовка/нижнего колонтитула."
type: docs
url: /ru/java/com.aspose.cells/headerfootercommand/
---

**Inheritance:**
java.lang.Object
```
public class HeaderFooterCommand
```

Представляет команду заголовка/нижнего колонтитула.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | Получает шрифт значения команды. |
| [getText()](#getText--) | Получает текст команды. |
| [getType()](#getType--) | Получает тип команды заголовка/нижнего колонтитула. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFont() {#getFont--}
```
public Font getFont()
```


Получает шрифт значения команды.

**Remarks**

Не используется для HeaderFooterCommandType.Picture.

**Returns:**
[Font](../../com.aspose.cells/font)
### getText() {#getText--}
```
public String getText()
```


Получает текст команды.

**Remarks**

Допустимо только для HeaderFooterCommandType.Text.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Получает тип команды заголовка/нижнего колонтитула.

См. [HeaderFooterCommandType](../../com.aspose.cells/headerfootercommandtype).

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

