---
title: "ChartCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/chartcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ChartCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [Chart](../../com.aspose.cells/chart).

**Example**

```
         Workbook workbook = new Workbook();
 
         ChartCollection charts = workbook.getWorksheets().get(0).getCharts();
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-byte---java.lang.String-boolean-int-int-int-int-) | Добавляет диаграмму с предустановленным шаблоном. |
| [add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)](#add-int-int-int-int-int-) | Добавляет диаграмму в коллекцию. |
| [add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-boolean-int-int-int-int-) | Добавляет диаграмму в коллекцию. |
| [add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)](#add-int-java.lang.String-int-int-int-int-) | Добавляет диаграмму в коллекцию. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [addFloatingChart(int type, int left, int top, int width, int height)](#addFloatingChart-int-int-int-int-int-) | Добавляет диаграмму в коллекцию. |
| [clear()](#clear--) | Очистить все диаграммы. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [Chart](../../com.aspose.cells/chart) по указанному индексу. |
| [get(String name)](#get-java.lang.String-) | Получает диаграмму по имени. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Chart chart)](#remove-com.aspose.cells.Chart-) | Удалить указанную диаграмму. |
| [removeAt(int index)](#removeAt-int-) | Удалить диаграмму по указанному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-byte---java.lang.String-boolean-int-int-int-int-}
```
public int add(byte[] data, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Добавляет диаграмму с предустановленным шаблоном.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| данные | byte[] | Данные файла шаблона диаграммы (.crtx). |
| dataRange | java.lang.String | Указывает диапазон данных диаграммы |
| isVertical | boolean | Указывает, строить ли ряды из диапазона значений ячеек по строкам или по столбцам. |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| rightRow | int | Индекс строки в нижнем правом углу |
| bottomColumn | int | Индекс столбца в нижнем правом углу |

**Returns:**
int — индекс объекта [Chart](../../com.aspose.cells/chart).
### add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn) {#add-int-int-int-int-int-}
```
public int add(int type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Добавляет диаграмму в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Тип диаграммы |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| bottomRow | int | Индекс строки в нижнем правом углу |
| rightColumn | int | Индекс столбца в нижнем правом углу |

**Returns:**
int — индекс объекта [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-boolean-int-int-int-int-}
```
public int add(int type, String dataRange, boolean isVertical, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Добавляет диаграмму в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Тип диаграммы |
| dataRange | java.lang.String | Указывает диапазон данных диаграммы |
| isVertical | boolean | Указывает, строить ли ряды из диапазона значений ячеек по строкам или по столбцам. |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| rightRow | int | Индекс строки в нижнем правом углу |
| bottomColumn | int | Индекс столбца в нижнем правом углу |

**Returns:**
int — индекс объекта [Chart](../../com.aspose.cells/chart).
### add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn) {#add-int-java.lang.String-int-int-int-int-}
```
public int add(int type, String dataRange, int topRow, int leftColumn, int rightRow, int bottomColumn)
```


Добавляет диаграмму в коллекцию.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство [add(int,String,boolean,int,int,int,int)](../../com.aspose.cells/chartcollection\#add-int-String-boolean-int-int-int-int-). Это свойство будет удалено через 12 месяцев, начиная с мая 2022 года. Компания Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Тип диаграммы |
| dataRange | java.lang.String | Указывает диапазон данных диаграммы |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| rightRow | int | Индекс строки в нижнем правом углу |
| bottomColumn | int | Индекс столбца в нижнем правом углу |

**Returns:**
int — индекс объекта [Chart](../../com.aspose.cells/chart).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### addFloatingChart(int type, int left, int top, int width, int height) {#addFloatingChart-int-int-int-int-int-}
```
public int addFloatingChart(int type, int left, int top, int width, int height)
```


Добавляет диаграмму в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ChartType](../../com.aspose.cells/charttype). Тип диаграммы |
| лево | int | Смещение по оси x до угла |
| верх | int | Смещение по оси y до угла |
| width | int | Ширина диаграммы |
| height | int | Высота диаграммы |

**Returns:**
int — индекс объекта [Chart](../../com.aspose.cells/chart).
### clear() {#clear--}
```
public void clear()
```


Очистить все диаграммы.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
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
### get(int index) {#get-int-}
```
public Chart get(int index)
```


Получает элемент [Chart](../../com.aspose.cells/chart) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public Chart get(String name)
```


Получает диаграмму по имени.

**Remarks**

Имя диаграммы по умолчанию равно null. Поэтому вам необходимо явно задать имя диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя диаграммы. |

**Returns:**
[Chart](../../com.aspose.cells/chart) - The chart.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Chart chart) {#remove-com.aspose.cells.Chart-}
```
public void remove(Chart chart)
```


Удалить указанную диаграмму.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| chart | [Chart](../../com.aspose.cells/chart) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удалить диаграмму по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс диаграммы. |

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

