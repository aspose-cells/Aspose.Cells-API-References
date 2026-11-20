---
title: "HorizontalPageBreakCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(int row)](#add-int-) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [add(int row, int column)](#add-int-int-) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | Добавляет горизонтальный разрыв страницы в коллекцию. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) по указанному индексу. |
| [get(String cellName)](#get-java.lang.String-) | Получает элемент [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) с указанным именем ячейки. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент HPageBreak с указанным именем. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


Добавляет горизонтальный разрыв страницы в коллекцию.

**Remarks**

Разрыв страницы добавляется в левый верхний угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки ячейки, начиная с нуля. |

**Returns:**
int — индекс объекта [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Добавляет горизонтальный разрыв страницы в коллекцию.

**Remarks**

Разрыв страницы добавляется в левый верхний угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки ячейки, начиная с нуля. |
| столбец | int | Индекс столбца ячейки, начиная с нуля. |

**Returns:**
int — индекс объекта [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


Добавляет горизонтальный разрыв страницы в коллекцию.

**Remarks**

Этот метод используется для добавления горизонтального разрыва страницы внутри области печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки, начиная с нуля. |
| startColumn | int | Индекс начального столбца, начиная с нуля. |
| endColumn | int | Индекс конечного столбца, начиная с нуля. |

**Returns:**
int — индекс объекта [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Добавляет горизонтальный разрыв страницы в коллекцию.

**Remarks**

Разрыв страницы добавляется в левый верхний угол ячейки. Пожалуйста, установите горизонтальный разрыв страницы и вертикальный разрыв страницы одновременно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |

**Returns:**
int — индекс объекта [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### clear() {#clear--}
```
public void clear()
```


Удаляет все объекты из экземпляра CollectionBase.

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
public HorizontalPageBreak get(int index)
```


Получает элемент [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


Получает элемент [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) с указанным именем ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | java.lang.String | Имя ячейки. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет элемент HPageBreak с указанным именем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс элемента, начиная с нуля. |

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

