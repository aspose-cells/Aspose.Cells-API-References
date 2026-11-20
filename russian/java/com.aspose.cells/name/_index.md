---
title: "Name"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет определённое имя для диапазона ячеек."
type: docs
url: /ru/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

Представляет определённое имя для диапазона ячеек.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Получает комментарий к имени. |
| [getFullText()](#getFullText--) | Получает полный текст имени объекта с настройкой области. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | Получает ссылку R1C1 на [Name](../../com.aspose.cells/name). |
| [getRange()](#getRange--) | Получает диапазон, если это имя ссылается на диапазон. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Получает диапазон, если это имя ссылается на диапазон |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Получает диапазон, если это имя ссылается на диапазон. |
| [getRanges()](#getRanges--) | Получает все диапазоны, на которые ссылается это имя. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Получает все диапазоны, на которые ссылается это имя. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Получает все ссылки, на которые ссылается это имя. |
| [getRefersTo()](#getRefersTo--) | Возвращает или задает формулу, к которой имя определено ссылаться, начиная со знака равенства. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Получить ссылку на это имя. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Получить ссылку на это имя, исходя из указанной ячейки. |
| [getSheetIndex()](#getSheetIndex--) | Указывает, к какой книге (Workbook) или листу (Worksheet) относится это имя. 0 = глобальное имя, иначе индекс листа (нумерация с 1). |
| [getText()](#getText--) | Получает текст имени объекта. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Указывает, используется ли это имя в других формулах. |
| [isVisible()](#isVisible--) | Указывает, видимо ли имя. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Устанавливает комментарий к имени. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | Устанавливает ссылку в формате R1C1 для [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | Возвращает или задает формулу, к которой имя определено ссылаться, начиная со знака равенства. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Установить ссылку для этого имени. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Указывает, к какой книге (Workbook) или листу (Worksheet) относится это имя. 0 = глобальное имя, иначе индекс листа (нумерация с 1). |
| [setText(String value)](#setText-java.lang.String-) | Получает текст имени объекта. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, видимо ли имя. |
| [toString()](#toString--) | Возвращает строку, представляющую текущий объект Range. |
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
### getComment() {#getComment--}
```
public String getComment()
```


Получает комментарий к имени. Применяется только к Excel 2007 и более новым версиям.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


Получает полный текст имени объекта с настройкой области.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


Получает ссылку R1C1 на [Name](../../com.aspose.cells/name).

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Получает диапазон, если это имя ссылается на диапазон.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


Получает диапазон, если это имя ссылается на диапазон

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пересчитать | boolean | нужно ли пересчитывать его, если это имя уже было вычислено до данного вызова. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


Получает диапазон, если это имя ссылается на диапазон. Если ссылка этого имени не абсолютна, диапазон может различаться для разных ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Соответствующий индекс листа. |
| строка | int | Соответствующий индекс строки. |
| столбец | int | Соответствующий индекс столбца |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Получает все диапазоны, на которые ссылается это имя.

**Returns:**
com.aspose.cells.Range[] - Все диапазоны.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


Получает все диапазоны, на которые ссылается это имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пересчитать | boolean | нужно ли пересчитывать его, если это имя уже было вычислено до данного вызова. |

**Returns:**
com.aspose.cells.Range[] - Все диапазоны.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


Получает все ссылки, на которые ссылается это имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пересчитать | boolean | нужно ли пересчитывать его, если это имя уже было вычислено до данного вызова. |

**Returns:**
com.aspose.cells.ReferredArea[] - Все диапазоны.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Возвращает или задает формулу, к которой имя определено ссылаться, начиная со знака равенства.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


Получить ссылку на это имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать ссылку как R1C1. |
| isLocal | boolean | Нужно ли форматировать ссылку в соответствии с локалью. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


Получить ссылку на это имя, исходя из указанной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать ссылку как R1C1. |
| isLocal | boolean | Нужно ли форматировать ссылку в соответствии с локалью. |
| строка | int | Индекс строки ячейки. |
| столбец | int | Индекс столбца ячейки. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Указывает, к какой книге (Workbook) или листу (Worksheet) относится это имя. 0 = глобальное имя, иначе индекс листа (нумерация с 1).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Получает текст имени объекта.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


Указывает, используется ли это имя в других формулах.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Указывает, видимо ли имя.

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




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Устанавливает комментарий к имени. Применяется только к Excel 2007 и более новым версиям.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


Устанавливает ссылку в формате R1C1 для [Name](../../com.aspose.cells/name).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


Возвращает или задает формулу, к которой имя определено ссылаться, начиная со знака равенства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


Установить ссылку для этого имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| refersTo | java.lang.String | Ссылка. |
| isR1C1 | boolean | Является ли ссылка форматом R1C1. |
| isLocal | boolean | Является ли ссылка отформатированной в соответствии с локалью. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


Указывает, к какой книге (Workbook) или листу (Worksheet) относится это имя. 0 = глобальное имя, иначе индекс листа (нумерация с 1).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Получает текст имени объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Указывает, видимо ли имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий объект Range.

**Returns:**
java.lang.String -
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

