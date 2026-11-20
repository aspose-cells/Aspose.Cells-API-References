---
title: "SheetRender"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет рендер листа, который может рендерить лист в различные изображения, такие как BMP, PNG, JPEG, TIFF.."
type: docs
url: /ru/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

Представляет рендер листа, который может рендерить лист в различные изображения, такие как (BMP, PNG, JPEG, TIFF..). Конструктор этого класса должен использоваться после изменения настройки страницы, стиля ячеек.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | конструктор SheetRender требует лист и ImageOrPrintOptions в качестве параметров |
## Методы

| Метод | Описание |
| --- | --- |
| [dispose()](#dispose--) | Освобождает ресурсы, созданные и используемые для рендеринга. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Получает общее количество страниц текущего листа. |
| [getPageScale()](#getPageScale--) | Получает вычисленный масштаб страницы листа. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Получить размер страницы в дюймах выходного изображения. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Отрендерить определённую страницу в поток. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Отрендерить определённую страницу в поток. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Отрендерить определённую страницу в файл. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Рендер листа на принтер |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Рендер листа на принтер |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Рендер листа на принтер |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | Рендер всего листа как TIFF‑изображение в поток. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


конструктор SheetRender требует лист и ImageOrPrintOptions в качестве параметров

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | Указывает, какая таблица должна быть отрендерена. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions содержит некоторые свойства выходного изображения |

### dispose() {#dispose--}
```
public void dispose()
```


Освобождает ресурсы, созданные и используемые для рендеринга.

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
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Получает общее количество страниц текущего листа.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


Получает вычисленный масштаб листа. Возвращает установленный масштаб, если установлен [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--). В противном случае возвращает вычисленный масштаб в соответствии с [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) и [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--).

**Example**

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         SheetRender sheetRender = new SheetRender(wb.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //Gets calculated page scale of the sheet.
         double pageScale = sheetRender.getPageScale();
```

**Returns:**
double
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


Получить размер страницы в дюймах выходного изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | int | Индекс страницы начинается с нуля. |

**Returns:**
float[] — размер изображения, [0] — ширина, [1] — высота
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




### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```


Отрендерить определённую страницу в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | int | укажите, какая страница будет конвертирована |
| stream | java.io.InputStream | поток выходного изображения |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


Отрендерить определённую страницу в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | int | укажите, какая страница будет конвертирована |
| stream | java.io.OutputStream | поток выходного изображения |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


Отрендерить определённую страницу в файл.

**Example**

Следующий код выводит первую страницу первого листа в PNG‑изображение.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
 
         //set output image type.
         imgOpt.setImageType(ImageType.PNG);
 
         //render the first sheet.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), imgOpt);
 
         //output the first page of the sheet to image.
         sr.toImage(0, "output.png");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | int | укажите, какая страница будет конвертирована |
| fileName | java.lang.String | имя файла выходного изображения |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Рендер листа на принтер

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | имя принтера, например: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Рендер листа на принтер

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте ToPrinter(string PrinterName) и ImageOrPrintOptions.PageIndex, PageCount для установки первой страницы и количества страниц для печати. Это свойство будет удалено через 12 месяцев, начиная с декабря 2021 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | имя принтера, например: "Microsoft Office Document Image Writer" |
| printPageIndex | int | нуль‑базовый индекс первой страницы для печати, он должен находиться в диапазоне [0, SheetRender.PageCount-1] |
| printPageCount | int | количество страниц для печати, оно должно быть больше нуля |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Рендер листа на принтер

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | имя принтера, например: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | установить имя задания печати |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


Рендер всего листа как TIFF‑изображение в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | поток выходного изображения |

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

