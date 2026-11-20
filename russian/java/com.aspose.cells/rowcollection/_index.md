---
title: "RowCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Собирает объекты, представляющие отдельные строки в листе."
type: docs
url: /ru/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Собирает объекты [Row](../../com.aspose.cells/row), представляющие отдельные строки в листе.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Методы

| Метод | Описание |
| --- | --- |
| [clear()](#clear--) | Очистить все строки и ячейки. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Получает объект [Row](../../com.aspose.cells/row) по заданному индексу строки. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество строк в этой коллекции. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Получает объект строки по позиции в списке. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Получает перечислитель, который перебирает строки в этой коллекции |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Получает перечислитель, который перебирает строки в этой коллекции |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент строки по указанному индексу (позиции) в этой коллекции. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Очистить все строки и ячейки.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Получает объект [Row](../../com.aspose.cells/row) по заданному индексу строки. Объект Row с указанным индексом будет создан, если он ранее не существовал.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


Получает количество строк в этой коллекции.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Получает объект строки по позиции в списке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Позиция. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает перечислитель, который перебирает строки в этой коллекции

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator — перечислитель строк, который будет проходить по всем существующим строкам в этой коллекции.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Получает перечислитель, который перебирает строки в этой коллекции

**Remarks**

Если коллекция строк будет изменена (операциями, которые могут привести к созданию новой Row или удалению существующей Row) во время обхода с помощью перечислителя, следует использовать синхронизированный перечислитель вместо обычного, чтобы обход мог продолжиться с позиции, следующей сразу после той, которую прошёл последний MoveNext(). Однако, помимо преимущества, что ни один элемент не будет пропущен или пройден несколько раз, недостатком синхронизированного перечислителя является небольшое снижение производительности по сравнению с обычным перечислителем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| обратный | boolean | нужно ли перечислять строки в обратном порядке |
| синхронный | boolean | нужно ли возвращаемому перечислителю проверять изменения коллекции строк и оставаться синхронным с ней. |

**Returns:**
java.util.Iterator — перечислитель строк, который будет проходить по всем существующим строкам в этой коллекции.
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


Удаляет элемент строки по указанному индексу (позиции) в этой коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | ноль‑базовый индекс (позиция, а не [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) существующего элемента строки в этой коллекции. |

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

