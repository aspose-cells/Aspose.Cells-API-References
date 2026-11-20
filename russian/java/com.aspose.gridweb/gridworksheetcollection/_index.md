---
title: "GridWorksheetCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

Инкапсулирует коллекцию объектов [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
## Методы

| Метод | Описание |
| --- | --- |
| [add()](#add--) | Добавляет лист в коллекцию. |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Добавляет лист в коллекцию. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [calculateFormula()](#calculateFormula--) | Вычисляет результат формул. |
| [clear()](#clear--) | Очистить все листы. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Получает элемент [GridWorksheet](../../com.aspose.gridweb/gridworksheet) по указанному индексу. |
| [get(String sheetName)](#get-java.lang.String-) | Получает элемент [GridWorksheet](../../com.aspose.gridweb/gridworksheet) с указанным именем. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Представляет индекс активного листа при открытии электронной таблицы. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает размер перечислителя |
| [getDefaultFontName()](#getDefaultFontName--) | Получает имя шрифта по умолчанию для элемента управления. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Получает коллекцию всех объектов Name в электронной таблице. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Получает десятичный разделитель для форматирования/разбора числовых значений. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Вставить лист. |
| [iterator()](#iterator--) | Получает перечислитель строк |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент по указанному индексу. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Удаляет элемент по указанному имени. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Представляет индекс активного листа при открытии электронной таблицы. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Устанавливает имя шрифта по умолчанию для элемента управления. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Устанавливает десятичный разделитель для форматирования/парсинга числовых значений. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Устанавливает видимость листа. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Обменивает местами два листа. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Добавляет лист в коллекцию.

**Returns:**
int — индекс объекта [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
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
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


Добавляет лист в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя листа |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Добавляет лист в коллекцию и копирует данные из существующего листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс исходного листа. |

**Returns:**
int — индекс объекта [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Добавляет лист в коллекцию и копирует данные из существующего листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя исходного листа. |

**Returns:**
int — индекс объекта [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Вычисляет результат формул.

### clear() {#clear--}
```
public void clear()
```


Очистить все листы.

**Remarks**

Книга должна содержать лист.

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
public GridWorksheet get(int index)
```


Получает элемент [GridWorksheet](../../com.aspose.gridweb/gridworksheet) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


Получает элемент [GridWorksheet](../../com.aspose.gridweb/gridworksheet) с указанным именем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя листа. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Представляет индекс активного листа при открытии электронной таблицы.

**Remarks**

Индекс листа начинается с нуля.

**Returns:**
int
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
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Получает имя шрифта по умолчанию для элемента управления.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


Получает коллекцию всех объектов Name в электронной таблице.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Получает десятичный разделитель для форматирования/парсинга числовых значений. По умолчанию используется десятичный разделитель текущего региона.

**Returns:**
char
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
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


Вставить лист.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс листа |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Получает перечислитель строк

**Returns:**
java.util.Iterator — перечислитель строк
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
| индекс | int | Значение индекса элемента, который нужно удалить. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Удаляет элемент по указанному имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя элемента, который нужно удалить. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Представляет индекс активного листа при открытии электронной таблицы.

**Remarks**

Индекс листа начинается с нуля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Устанавливает имя шрифта по умолчанию для элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Устанавливает десятичный разделитель для форматирования/парсинга числовых значений. По умолчанию используется десятичный разделитель текущего региона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


Устанавливает видимость листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя исходного листа. |
| isVisible | boolean | Является ли лист видимым |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Обменивает местами два листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex1 | int | Первый лист. |
| sheetIndex2 | int | Второй лист. |

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

