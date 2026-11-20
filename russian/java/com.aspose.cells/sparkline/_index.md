---
title: "Спарклайн"
second_title: "Справочник API Aspose.Cells for Java"
description: "Спарклайн представляет собой крошечную диаграмму или графику в ячейке листа, предоставляющую визуальное представление данных."
type: docs
url: /ru/java/com.aspose.cells/sparkline/
---

**Inheritance:**
java.lang.Object
```
public class Sparkline
```

Спарклайн представляет собой крошечную диаграмму или графику в ячейке листа, предоставляющую визуальное представление данных.

**Example**

```
         Workbook book = new Workbook(); 
         Worksheet sheet = book.getWorksheets().get(0);
 
         sheet.getCells().get("A1").putValue(5);
         sheet.getCells().get("B1").putValue(2);
         sheet.getCells().get("C1").putValue(1);
         sheet.getCells().get("D1").putValue(3);
 
         // Define the CellArea
         CellArea ca = new CellArea();
         ca.StartColumn = 4;
         ca.EndColumn = 4;
         ca.StartRow = 0;
         ca.EndRow = 0;
 
         int idx = sheet.getSparklineGroups().add(com.aspose.cells.SparklineType.LINE, sheet.getName() + "!A1:D1", false, ca);
 
         SparklineGroup group = sheet.getSparklineGroups().get(idx);
         idx = group.getSparklines().add(sheet.getName() + "!A1:D1", 0, 4);
         Sparkline line = group.getSparklines().get(idx);
         System.out.println("Saprkline data range: " + line.getDataRange() + ", row: " + line.getRow() + ", column: " + line.getColumn());
         line.toImage("output.png", new ImageOrPrintOptions());
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Получает индекс столбца спарклайна. |
| [getDataRange()](#getDataRange--) | Представляет диапазон данных спарклайна. |
| [getRow()](#getRow--) | Получает индекс строки спарклайна. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataRange(String value)](#setDataRange-java.lang.String-) | Представляет диапазон данных спарклайна. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Преобразует спарклайн в изображение. |
| [toImage(String fileName, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Преобразует спарклайн в изображение. |
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
### getColumn() {#getColumn--}
```
public int getColumn()
```


Получает индекс столбца спарклайна.

**Returns:**
int
### getDataRange() {#getDataRange--}
```
public String getDataRange()
```


Представляет диапазон данных спарклайна.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Получает индекс строки спарклайна.

**Returns:**
int
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




### setDataRange(String value) {#setDataRange-java.lang.String-}
```
public void setDataRange(String value)
```


Представляет диапазон данных спарклайна.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Преобразует спарклайн в изображение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток изображения. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Параметры изображения. |

### toImage(String fileName, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String fileName, ImageOrPrintOptions options)
```


Преобразует спарклайн в изображение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла изображения. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Параметры изображения |

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

