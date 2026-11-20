---
title: "GridHyperlinkCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

Инкапсулирует коллекцию объектов [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
## Методы

| Метод | Описание |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Добавляет гиперссылку в указанную ячейку. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [clear()](#clear--) | Очищает все гиперссылки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает размер перечислителя |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Получает объект Hyperlink ячейки. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Получает объект Hyperlink ячейки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Удаляет гиперссылку в указанной области. |
| [removeAt(int index)](#removeAt-int-) | Удаляет гиперссылку по указанному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка диапазона гиперссылок. |
| firstColumn | int | Первый столбец диапазона гиперссылок. |
| totalRows | int | Количество строк в этом диапазоне гиперссылок. |
| totalColumns | int | Количество столбцов этого диапазона гиперссылок. |
| адрес | java.lang.String | Адрес гиперссылки. |

**Returns:**
int - индекс объекта [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |
| totalRows | int | Количество строк в этом диапазоне гиперссылок. |
| totalColumns | int | Количество столбцов этого диапазона гиперссылок. |
| адрес | java.lang.String | Адрес гиперссылки. |

**Returns:**
int - индекс объекта [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


Добавляет гиперссылку в указанную ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |
| адрес | java.lang.String | Адрес гиперссылки. |

**Returns:**
int - индекс объекта [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startCellName | java.lang.String | Верхняя‑левая ячейка диапазона. |
| endCellName | java.lang.String | Ячейка диапазона в правом нижнем углу. |
| адрес | java.lang.String | Адрес гиперссылки. |
| textToDisplay | java.lang.String | Текст, который будет отображаться для указанной гиперссылки. |
| screenTip | java.lang.String | Текст подсказки (screenTip) для указанной гиперссылки. |

**Returns:**
int - индекс объекта [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### clear() {#clear--}
```
public void clear()
```


Очищает все гиперссылки.

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
public GridHyperlink get(int index)
```


Получает элемент [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
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


Получает размер перечислителя

**Returns:**
int
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


Получает объект Hyperlink ячейки. Если у ячейки нет Hyperlink, возвращает null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | Объект GridCell. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


Получает объект Hyperlink ячейки. Если у ячейки нет Hyperlink, возвращает null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Строка ячейки. |
| столбец | int | Столбец ячейки. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


Удаляет гиперссылку в указанной области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Область, содержащая гиперссылку. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет гиперссылку по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

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

