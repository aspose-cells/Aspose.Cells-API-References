---
title: "ReConnectionMethodType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Указывает, что должно делать приложение электронной таблицы при сбое соединения."
type: docs
url: /ru/java/com.aspose.cells/reconnectionmethodtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```

Указывает, что должно делать приложение электронной таблицы при сбое соединения.
## Поля

| Поле | Описание |
| --- | --- |
| [ALWAYS](#ALWAYS) | При каждом обновлении получать обновлённую информацию о соединении из внешнего файла соединения, если он доступен, и использовать её вместо существующей информации о соединении. |
| [NEVER](#NEVER) | Никогда не получать обновлённую информацию о соединении из внешнего файла соединения, даже если он доступен и даже если существующая информация о соединении недействительна. |
| [REQUIRED](#REQUIRED) | При обновлении использовать существующую информацию о соединении, и если она окажется недействительной, тогда получить обновлённую информацию о соединении, если она доступна во внешнем файле соединения. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


При каждом обновлении получать обновлённую информацию о соединении из внешнего файла соединения, если он доступен, и использовать её вместо существующей информации о соединении. В этом случае обновление данных завершится неудачей, если внешний файл соединения недоступен.

### NEVER {#NEVER}
```
public static final int NEVER
```


Никогда не получать обновлённую информацию о соединении из внешнего файла соединения, даже если он доступен и даже если существующая информация о соединении недействительна.

### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```


При обновлении использовать существующую информацию о соединении, и если она окажется недействительной, тогда получить обновлённую информацию о соединении, если она доступна во внешнем файле соединения.

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

