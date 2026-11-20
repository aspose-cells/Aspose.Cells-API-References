---
title: "RenameStrategy"
second_title: "Справочник API Aspose.Cells for Java"
description: "Вариант стратегии для дублирующихся имен столбцов."
type: docs
url: /ru/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

Вариант стратегии для дублирующихся имен столбцов.

**Remarks**

При обработке данных с заголовками в некоторых сценариях требуется отсутствие дублирования заголовков для всех столбцов. Например, при экспорте данных в datatable и когда заголовок должен использоваться в качестве имени столбца datatable, дублирующиеся значения заголовка недопустимы. Для таких ситуаций пользователь может определить, как их обрабатывать, указав эту стратегию.
## Поля

| Поле | Описание |
| --- | --- |
| [DIGIT](#DIGIT) | Имя содержит цифру. |
| [EXCEPTION](#EXCEPTION) | Выбрасывает исключение. |
| [LETTER](#LETTER) | Имя содержит букву.. |
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
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


Имя содержит цифру. Дублированные имена будут преобразованы в ...1, ...2 и т.д.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


Выбрасывает исключение.

### LETTER {#LETTER}
```
public static final int LETTER
```


Имя содержит букву.. Дублированные имена будут преобразованы в ...A, ...B и т.д.

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

