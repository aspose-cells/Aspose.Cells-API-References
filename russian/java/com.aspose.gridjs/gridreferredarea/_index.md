---
title: "GridReferredArea"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет ссылочную область по формуле."
type: docs
url: /ru/java/com.aspose.gridjs/gridreferredarea/
---

**Inheritance:**
java.lang.Object
```
public class GridReferredArea
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
| [getSheetName()](#getSheetName--) | Указывает, в каком листе это находится |
| [getStartColumn()](#getStartColumn--) | Начальный столбец области. |
| [getStartRow()](#getStartRow--) | Начальная строка области. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Получает значение ячейки с заданным смещением от верхнего левого угла этой области. |
| [getValues()](#getValues--) | Получает значения ячеек в этой области. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Указывает, является ли это областью. |
| [isExternalLink()](#isExternalLink--) | Указывает, является ли это внешней ссылкой. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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


Указывает, в каком листе это находится

**Returns:**
java.lang.String
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
### getValues() {#getValues--}
```
public Object getValues()
```


Получает значения ячеек в этой области.

**Returns:**
java.lang.Object — Если эта область недействительна, будет возвращено "\#REF!"; Если область состоит из одной ячейки, вернуть объект значения ячейки; В противном случае вернуть массив со всеми значениями в этой области.
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

