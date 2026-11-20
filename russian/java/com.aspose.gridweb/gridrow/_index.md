---
title: "GridRow"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий отдельное изображение в электронных таблицах."
type: docs
url: /ru/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

Инкапсулирует объект, представляющий отдельное изображение в электронных таблицах.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Получает ячейку. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Получить ячейку по конкретному индексу в списке. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Получает первую ячейку в строке. |
| [getHeight()](#getHeight--) | Получает высоту строки в единицах Points. |
| [getHidden()](#getHidden--) | Указывает, скрыта ли строка. |
| [getIndex()](#getIndex--) | Получает индекс этой строки. |
| [getLastCell()](#getLastCell--) | Получает последнюю ячейку в строке. |
| [getLastDataCell()](#getLastDataCell--) | Получает последнюю ячейку в строке. |
| [getOutlineLevel()](#getOutlineLevel--) | Получает уровень структуры. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Указывает, содержит ли строка какие-либо данные |
| [iterator()](#iterator--) | Получает перечислитель ячеек |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Устанавливает высоту строки в единицах точек. |
| [setHidden(boolean value)](#setHidden-boolean-) | Указывает, скрыта ли строка. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Устанавливает уровень структуры. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


Получает ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| столбец | int | Индекс столбца |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


Получить ячейку по конкретному индексу в списке.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Row.GetEnumerator() для перебора всех ячеек в этой строке. Это свойство будет удалено через 12 месяцев, начиная с февраля 2015 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Позиция. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Получает первую ячейку в строке.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


Получает высоту строки в единицах Points.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


Указывает, скрыта ли строка.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает индекс этой строки.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Получает последнюю ячейку в строке.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


Получает последнюю ячейку в строке.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


Получает уровень структуры.

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Указывает, содержит ли строка какие-либо данные

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает перечислитель ячеек

**Returns:**
java.util.Iterator - Enumerator ячеек
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Устанавливает высоту строки в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Указывает, скрыта ли строка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


Устанавливает уровень структуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte |  |

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

