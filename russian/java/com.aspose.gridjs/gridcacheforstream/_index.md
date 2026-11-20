---
title: "GridCacheForStream"
second_title: "Справочник API Aspose.Cells for Java"
description: "Этот класс содержит операции кэша для GridJs."
type: docs
url: /ru/java/com.aspose.gridjs/gridcacheforstream/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```

Этот класс содержит операции кэша для GridJs. Пользователь должен реализовать собственную бизнес-логику хранения на его основе..
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Реализует этот метод для получения file url из кэша. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | Проверяет, существует ли кэш с uid |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Реализует этот метод для загрузки кэша по ключу uid, возвращает поток из кэша. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Реализует этот метод для сохранения кэша, сохраняет поток в кэш по ключу uid. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridCacheForStream() {#GridCacheForStream--}
```
public GridCacheForStream()
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
### getFileUrl(String uid) {#getFileUrl-java.lang.String-}
```
public abstract String getFileUrl(String uid)
```


Реализует этот метод для получения file url из кэша.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
java.lang.String - URL файла
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExisted(String uid) {#isExisted-java.lang.String-}
```
public abstract boolean isExisted(String uid)
```


Проверяет, существует ли кэш с uid

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для кэша файла. |

**Returns:**
boolean - логическое значение
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```


Реализует этот метод для загрузки кэша по ключу uid, возвращает поток из кэша.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
java.io.InputStream
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveStream(InputStream s, String uid) {#saveStream-java.io.InputStream-java.lang.String-}
```
public abstract void saveStream(InputStream s, String uid)
```


Реализует этот метод для сохранения кэша, сохраняет поток в кэш по ключу uid.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| s | java.io.InputStream |  |
| uid | java.lang.String |  |

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

