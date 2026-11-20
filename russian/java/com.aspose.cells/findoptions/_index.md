---
title: "FindOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры поиска."
type: docs
url: /ru/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Представляет параметры поиска.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Указывает, чувствителен ли поиск к регистру строки. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Получает значение, указывающее, следует ли преобразовать найденную строку в числовые данные. |
| [getLookAtType()](#getLookAtType--) | Тип LookAt. |
| [getLookInType()](#getLookInType--) | Тип LookIn. |
| [getRange()](#getRange--) | Получает и задает диапазон поиска. |
| [getRegexKey()](#getRegexKey--) | Указывает, является ли искомый ключ регулярным выражением. |
| [getSearchBackward()](#getSearchBackward--) | Искать ячейки в обратном порядке. |
| [getSearchNext()](#getSearchNext--) | Порядок поиска. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Указывает, осуществляется ли порядок поиска по строкам или столбцам. |
| [getStyle()](#getStyle--) | Формат для поиска. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Указывает, должен ли тип значения найденной ячейки совпадать с типом искомого ключа. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Указывает, установлен ли искомый диапазон. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Указывает, чувствителен ли поиск к регистру строки. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Устанавливает значение, указывающее, следует ли преобразовывать найденное строковое значение в числовые данные. |
| [setLookAtType(int value)](#setLookAtType-int-) | Тип LookAt. |
| [setLookInType(int value)](#setLookInType-int-) | Тип LookIn. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Устанавливает искомый диапазон. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Указывает, является ли искомый ключ регулярным выражением. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Искать ячейки в обратном порядке. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Порядок поиска. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Указывает, осуществляется ли порядок поиска по строкам или столбцам. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Формат для поиска. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Указывает, должен ли тип значения найденной ячейки совпадать с типом искомого ключа. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Указывает, чувствителен ли поиск к регистру строки.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Получает значение, указывающее, следует ли преобразовать найденную строку в числовые данные.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Тип LookAt.

Смотрите [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Когда [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) возвращает true и пользователь указал точное правило для regex, с точки зрения производительности это свойство следует установить как [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). В противном случае мы будем преобразовывать ключ поиска, чтобы обеспечить соответствие конкретному типу. Например, когда тип равен [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (это значение по умолчанию для этого свойства), мы автоматически добавим подстановочные символы в начало и конец ключа поиска. В этом случае регулярные выражения станут более сложными, и производительность также снизится.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


Тип LookIn.

Смотрите [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


Получает и задает диапазон поиска.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


Указывает, является ли искомый ключ регулярным выражением. Если true, ключ будет восприниматься как regex и анализироваться. В противном случае ключ будет анализироваться согласно правилам MS Excel.

**Remarks**

Несмотря на то, что ключ поиска указан как regex, он может быть преобразован в соответствии с указанным [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). Например, когда тип равен [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (это значение по умолчанию для этих параметров), подстановочные символы автоматически добавляются в начало и конец ключа поиска, чтобы проверка соответствия выполнялась как "contains". В этом случае регулярные выражения становятся более сложными, и производительность также снижается. Поэтому, с точки зрения производительности, если пользователь указал точное правило для regex, нет необходимости использовать [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) в качестве дополнительного ограничения, и пользователь может установить его как [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) для лучшей производительности.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


Искать ячейки в обратном порядке.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


Порядок поиска. True: искать следующий. False: искать предыдущий.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FindOptions.SearchBackward. Это свойство будет удалено через 12 месяцев, начиная с ноября 2018 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


Указывает, осуществляется ли порядок поиска по строкам или столбцам.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Формат для поиска.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


Указывает, должен ли тип значения найденной ячейки совпадать с типом искомого ключа.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


Указывает, установлен ли искомый диапазон.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Указывает, чувствителен ли поиск к регистру строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Устанавливает значение, указывающее, следует ли преобразовывать найденное строковое значение в числовые данные.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


Тип LookAt.

Смотрите [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Когда [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) возвращает true и пользователь указал точное правило для regex, с точки зрения производительности это свойство следует установить как [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). В противном случае мы будем преобразовывать ключ поиска, чтобы обеспечить соответствие конкретному типу. Например, когда тип равен [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (это значение по умолчанию для этого свойства), мы автоматически добавим подстановочные символы в начало и конец ключа поиска. В этом случае регулярные выражения станут более сложными, и производительность также снизится.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


Тип LookIn.

Смотрите [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


Устанавливает искомый диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | искомый диапазон. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


Указывает, является ли искомый ключ регулярным выражением. Если true, ключ будет восприниматься как regex и анализироваться. В противном случае ключ будет анализироваться согласно правилам MS Excel.

**Remarks**

Несмотря на то, что ключ поиска указан как regex, он может быть преобразован в соответствии с указанным [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). Например, когда тип равен [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (это значение по умолчанию для этих параметров), подстановочные символы автоматически добавляются в начало и конец ключа поиска, чтобы проверка соответствия выполнялась как "contains". В этом случае регулярные выражения становятся более сложными, и производительность также снижается. Поэтому, с точки зрения производительности, если пользователь указал точное правило для regex, нет необходимости использовать [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) в качестве дополнительного ограничения, и пользователь может установить его как [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) для лучшей производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


Искать ячейки в обратном порядке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


Порядок поиска. True: искать следующий. False: искать предыдущий.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FindOptions.SearchBackward. Это свойство будет удалено через 12 месяцев, начиная с ноября 2018 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


Указывает, осуществляется ли порядок поиска по строкам или столбцам.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Формат для поиска.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


Указывает, должен ли тип значения найденной ячейки совпадать с типом искомого ключа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

