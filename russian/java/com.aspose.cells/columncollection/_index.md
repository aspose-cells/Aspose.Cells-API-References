---
title: "ColumnCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Коллекция объектов, представляющих отдельные настройки столбцов в листе."
type: docs
url: /ru/java/com.aspose.cells/columncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ColumnCollection extends CollectionBase
```

Коллекция объектов [Column](../../com.aspose.cells/column), представляющих отдельные настройки столбцов в листе. Объект Column представляет только такие настройки, как ширина столбца, стили и т.д. для всего столбца и не имеет отношения к наличию или отсутствию непустых ячеек (данных) в соответствующем столбце. А свойство "Count" этой коллекции отражает лишь количество созданных в ней объектов Column и не связано с тем, есть ли в листе непустые ячейки (данные).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add new Style to Workbook
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setForegroundColor(Color.getBlue());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.SOLID);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Change the default width of first ten columns
         for (int i = 0; i ? i++)
         {
             worksheet.getCells().getColumns().get(i).setWidth(20);
         }
 
         //Get the Column with non default formatting
         ColumnCollection columns = worksheet.getCells().getColumns();
 
         for (Column column : (Iterable<Column>) columns)
         {
             //Apply Style to first ten Columns
             column.applyStyle(style, styleFlag);
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int columnIndex)](#get-int-) | Получает объект [Column](../../com.aspose.cells/column) по индексу столбца. |
| [getByIndex(int index)](#getByIndex-int-) | Получает объект столбца по индексу. |
| [getClass()](#getClass--) |  |
| [getColumnByIndex(int index)](#getColumnByIndex-int-) | Получает объект [Column](../../com.aspose.cells/column) по позиции в списке. |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент по указанному индексу. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### get(int columnIndex) {#get-int-}
```
public Column get(int columnIndex)
```


Получает объект [Column](../../com.aspose.cells/column) по индексу столбца. Объект Column для указанного индекса столбца будет создан, если он ранее не существовал.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int |  |

**Returns:**
[Column](../../com.aspose.cells/column)
### getByIndex(int index) {#getByIndex-int-}
```
public Column getByIndex(int index)
```


Получает объект столбца по индексу.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Columns.GetColumnByIndex(). Это свойство будет удалено через 12 месяцев, начиная с июня 2010 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int |  |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnByIndex(int index) {#getColumnByIndex-int-}
```
public Column getColumnByIndex(int index)
```


Получает объект [Column](../../com.aspose.cells/column) по позиции в списке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Позиция в списке. |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
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


Удаляет элемент по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента, который нужно удалить. |

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

