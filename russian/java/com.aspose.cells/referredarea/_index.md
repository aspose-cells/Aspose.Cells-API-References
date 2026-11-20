---
title: "ReferredArea"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет ссылочную область по формуле."
type: docs
url: /ru/java/com.aspose.cells/referredarea/
---

**Inheritance:**
java.lang.Object
```
public class ReferredArea
```

Представляет ссылочную область по формуле.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Конечный столбец области. |
| [getEndRow()](#getEndRow--) | Конечная строка области. |
| [getExternalFileName()](#getExternalFileName--) | Получить имя внешнего файла, если это внешняя ссылка. |
| [getSheetName()](#getSheetName--) | Указывает, в каком листе находится эта ссылка. |
| [getSheetNames()](#getSheetNames--) | Имена всех листов, на которые ссылается этот экземпляр. |
| [getStartColumn()](#getStartColumn--) | Начальный столбец области. |
| [getStartRow()](#getStartRow--) | Начальная строка области. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Получает значение ячейки с заданным смещением от верхнего левого угла этой области. |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | Получает значение ячейки с заданным смещением от верхнего левого угла этой области. |
| [getValues()](#getValues--) | Получает значения ячеек в этой области. |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | Получает значения ячеек в этой области. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Указывает, является ли это областью. |
| [isEntireColumn()](#isEntireColumn--) | Указывает, содержит ли эта область все строки (полный столбец). |
| [isEntireRow()](#isEntireRow--) | Указывает, содержит ли эта область все столбцы (полная строка). |
| [isExternalLink()](#isExternalLink--) | Указывает, является ли это внешней ссылкой. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Возвращает адрес ссылки этой области. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Конечный столбец области.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Конечная строка области.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


Получить имя внешнего файла, если это внешняя ссылка.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Указывает, в каком листе находится эта ссылка.

**Remarks**

Если она ссылается на несколько листов, возвращаемое значение выглядит как выражение диапазона в формуле. Например "Sheet1:Sheet3" для ссылки в формуле "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```


Имена всех листов, на которые ссылается этот экземпляр.

**Returns:**
java.lang.String[]
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Начальный столбец области.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Начальная строка области.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Получает значение ячейки с заданным смещением от верхнего левого угла этой области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | смещение строки от начальной строки этой области |
| colOffset | int | смещение столбца от начальной строки этой области |

**Returns:**
java.lang.Object - "\#REF!" если эта область недействительна; "\#N/A" если заданное смещение выходит за пределы этой области; иначе возвращает значение ячейки в указанной позиции.
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```


Получает значение ячейки с заданным смещением от верхнего левого угла этой области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | int | смещение строки от начальной строки этой области |
| colOffset | int | смещение столбца от начальной строки этой области |
| calculateFormulas | boolean | Нужно ли вычислять её рекурсивно, если указанная ссылка является формулой |

**Returns:**
java.lang.Object - "\#REF!" если эта область недействительна; "\#N/A" если заданное смещение выходит за пределы этой области; иначе возвращает значение ячейки в указанной позиции.
### getValues() {#getValues--}
```
public Object getValues()
```


Получает значения ячеек в этой области.

**Returns:**
java.lang.Object - Если эта область недействительна, будет возвращено "\#REF!"; если область состоит из одной ячейки, возвращается объект значения ячейки; иначе возвращается двумерный массив со всеми значениями в этой области.
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```


Получает значения ячеек в этой области.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| calculateFormulas | boolean | В этом диапазоне, если есть формулы, которые не были вычислены, этот флаг указывает, следует ли вычислять эти формулы рекурсивно |

**Returns:**
java.lang.Object - Если эта область недействительна, будет возвращено "\#REF!"; если область состоит из одной ячейки, возвращается объект значения ячейки; иначе возвращается двумерный массив со всеми значениями в этой области.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Указывает, является ли это областью.

**Remarks**

Если это не область, действуют только StartRow и StartColumn.

**Returns:**
boolean
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```


Указывает, содержит ли эта область все строки (полный столбец).

**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```


Указывает, содержит ли эта область все столбцы (полная строка).

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Указывает, является ли это внешней ссылкой.

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




### toString() {#toString--}
```
public String toString()
```


Возвращает адрес ссылки этой области. Обычно это адрес ссылки, который может использоваться в формуле, например "Sheet1!A1:C3".

**Returns:**
java.lang.String - адрес ссылки этой области.
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

