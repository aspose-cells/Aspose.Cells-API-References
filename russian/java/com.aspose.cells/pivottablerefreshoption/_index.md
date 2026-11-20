---
title: "PivotTableRefreshOption"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры обновления источника данных сводной таблицы."
type: docs
url: /ru/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

Представляет параметры обновления источника данных сводной таблицы.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | Представляет параметры обновления источника данных сводной таблицы. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | Указывает, следует ли сохранять кэшированные локальные групповые данные, если максимальные и минимальные значения остаются неизменными. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Представляет способ резервирования отсутствующих элементов сводной таблицы. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | Указывает, следует ли сохранять оригинальный порядок элементов сводной таблицы как в старом источнике данных. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | Указывает, следует ли сохранять кэшированные локальные групповые данные, если максимальные и минимальные значения остаются неизменными. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | Указывает, следует ли сохранять оригинальный порядок элементов сводной таблицы как в старом источнике данных. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Представляет способ резервирования отсутствующих элементов сводной таблицы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


Представляет параметры обновления источника данных сводной таблицы.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


Указывает, следует ли сохранять кэшированные локальные групповые данные, если максимальные и минимальные значения остаются неизменными. Значение по умолчанию — false, что означает обновление группы с локальными настройками.

**Remarks**

Это временное решение, пожалуйста, локализуйте сводные таблицы, реализовав [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Представляет способ резервирования отсутствующих элементов сводной таблицы.

Смотрите [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


Указывает, следует ли сохранять оригинальный порядок элементов сводной таблицы как в старом источнике данных.

**Remarks**

Применяется только к полю сводной таблицы, которое не отсортировано. При обновлении такого поля Ms Excel сохраняет оригинальный порядок старого источника данных. Значение свойства по умолчанию — true, что соответствует поведению Ms Excel. Если пользователю необходимо полностью обновить поле сводной таблицы в соответствии с данными нового источника, это свойство следует установить в false.

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




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


Указывает, следует ли сохранять кэшированные локальные групповые данные, если максимальные и минимальные значения остаются неизменными. Значение по умолчанию — false, что означает обновление группы с локальными настройками.

**Remarks**

Это временное решение, пожалуйста, локализуйте сводные таблицы, реализовав [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


Указывает, следует ли сохранять оригинальный порядок элементов сводной таблицы как в старом источнике данных.

**Remarks**

Применяется только к полю сводной таблицы, которое не отсортировано. При обновлении такого поля Ms Excel сохраняет оригинальный порядок старого источника данных. Значение свойства по умолчанию — true, что соответствует поведению Ms Excel. Если пользователю необходимо полностью обновить поле сводной таблицы в соответствии с данными нового источника, это свойство следует установить в false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Представляет способ резервирования отсутствующих элементов сводной таблицы.

Смотрите [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

