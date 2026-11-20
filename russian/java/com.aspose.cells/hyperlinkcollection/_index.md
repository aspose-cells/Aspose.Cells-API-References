---
title: "HyperlinkCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/hyperlinkcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HyperlinkCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [Hyperlink](../../com.aspose.cells/hyperlink).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Get Hyperlinks Collection
         HyperlinkCollection hyperlinks = worksheet.getHyperlinks();
 
         //Adding a hyperlink to a URL at "A1" cell
         hyperlinks.add("A1", 1, 1, "http://www.aspose.com");
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [clear()](#clear--) | Очищает все гиперссылки. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [Hyperlink](../../com.aspose.cells/hyperlink) по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет гиперссылку по указанному индексу в этой коллекции. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook();
         Worksheet worksheet = excel.getWorksheets().get(0);
         worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
         worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | int | Первая строка диапазона гиперссылок. |
| firstColumn | int | Первый столбец диапазона гиперссылок. |
| totalRows | int | Количество строк в этом диапазоне гиперссылок. |
| totalColumns | int | Количество столбцов этого диапазона гиперссылок. |
| адрес | java.lang.String | Адрес гиперссылки. |

**Returns:**
int — индекс объекта [Hyperlink](../../com.aspose.cells/hyperlink).
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
int — индекс объекта [Hyperlink](../../com.aspose.cells/hyperlink).
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
int — индекс объекта [Hyperlink](../../com.aspose.cells/hyperlink).
### clear() {#clear--}
```
public void clear()
```


Очищает все гиперссылки.

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
public Hyperlink get(int index)
```


Получает элемент [Hyperlink](../../com.aspose.cells/hyperlink) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - The element at the specified index.
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


Удаляет гиперссылку по указанному индексу в этой коллекции.

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

