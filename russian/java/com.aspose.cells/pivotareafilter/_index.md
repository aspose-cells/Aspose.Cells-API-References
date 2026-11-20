---
title: "PivotAreaFilter"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет фильтр  для ."
type: docs
url: /ru/java/com.aspose.cells/pivotareafilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotAreaFilter
```

Представляет фильтр [PivotArea](../../com.aspose.cells/pivotarea) для [PivotTable](../../com.aspose.cells/pivottable).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotAreaFilter()](#PivotAreaFilter--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Получает индекс поля в исходных полях, к которому относится этот фильтр. |
| [getSelected()](#getSelected--) | Указывает, имеет ли это поле выделение. |
| [hashCode()](#hashCode--) |  |
| [isSubtotalSet(int subtotalType)](#isSubtotalSet-int-) | Получает, какой промежуточный итог установлен для этого фильтра. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setSelected(boolean value)](#setSelected-boolean-) | Указывает, имеет ли это поле выделение. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Промежуточный итог для фильтра. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotAreaFilter() {#PivotAreaFilter--}
```
public PivotAreaFilter()
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
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Получает индекс поля в исходных полях, к которому относится этот фильтр. Значение -2 указывает на поле значений.

**Returns:**
int
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Указывает, имеет ли это поле выделение. Работает только когда сводная таблица находится в режиме структуры.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSubtotalSet(int subtotalType) {#isSubtotalSet-int-}
```
public boolean isSubtotalSet(int subtotalType)
```


Получает, какой промежуточный итог установлен для этого фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Тип функции промежуточного итога. |

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Указывает, имеет ли это поле выделение. Работает только когда сводная таблица находится в режиме структуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Промежуточный итог для фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Функция промежуточного итога. |
| показано | boolean | Указывает, отображаются ли эти данные промежуточного итога. |

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

