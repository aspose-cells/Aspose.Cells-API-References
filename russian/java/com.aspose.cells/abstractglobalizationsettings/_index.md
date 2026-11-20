---
title: "AbstractGlobalizationSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройки глобализации."
type: docs
url: /ru/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

Представляет настройки глобализации.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Сравнивает две строковые величины согласно определённым правилам сортировки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Преобразует строку в сравнимый объект согласно определённым правилам сортировки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Сравнивает две строковые величины согласно определённым правилам сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| v1 | java.lang.String | первая строка |
| v2 | java.lang.String | вторая строка |
| ignoreCase | boolean | нужно ли игнорировать регистр при сравнении значений |

**Returns:**
int — целое число, указывающее лексическое отношение между двумя сравниваемыми значениями
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Преобразует строку в сравнимый объект согласно определённым правилам сортировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| v | java.lang.String | Значение String должно сравниваться с другими. |
| ignoreCase | boolean | нужно ли игнорировать регистр при сравнении значений |

**Returns:**
java.lang.Comparable - Объект может использоваться для сравнения или сортировки строковых значений.
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

