---
title: "WorkbookRender"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет рендер рабочей книги."
type: docs
url: /ru/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

Представляет рендеринг Workbook. Конструктор этого класса должен использоваться после изменения параметров страницы и стиля ячеек.

**Remarks**
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | Конструктор WorkbookRender |
## Методы

| Метод | Описание |
| --- | --- |
| [dispose()](#dispose--) | Освобождает ресурсы, созданные и используемые для рендеринга. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Получает общее количество страниц рабочей книги. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Получить размер страницы в дюймах выходного изображения. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Отрендерить определённую страницу в поток. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Отрендерить определённую страницу в поток. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Отрендерить определённую страницу в файл. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Отрендерить всю рабочую книгу как TIFF‑изображение в поток. |
| [toImage(String filename)](#toImage-java.lang.String-) | Отрендерить всю рабочую книгу как TIFF‑изображение в файл. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Отрендерить рабочую книгу на принтер |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Отрендерить рабочую книгу на принтер |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Отрендерить рабочую книгу на принтер |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


Конструктор WorkbookRender

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Укажите, какая рабочая книга будет отрендерена. |
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


Получает общее количество страниц рабочей книги.

**Returns:**
int
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

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | int | укажите, какая страница будет конвертирована |
| fileName | java.lang.String | имя файла выходного изображения |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


Отрендерить всю рабочую книгу как TIFF‑изображение в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | поток выходного изображения |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


Отрендерить всю рабочую книгу как TIFF‑изображение в файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filename | java.lang.String | имя файла выходного изображения |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Отрендерить рабочую книгу на принтер

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | имя принтера, например: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Отрендерить рабочую книгу на принтер

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте ToPrinter(string PrinterName) и ImageOrPrintOptions.PageIndex, PageCount для установки первой страницы и количества страниц для печати. Это свойство будет удалено через 12 месяцев, начиная с декабря 2021 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String | имя принтера, например: "Microsoft Office Document Image Writer" |
| printPageIndex | int | нуль‑базовый индекс первой страницы для печати, он должен находиться в диапазоне [0, WorkbookRender.PageCount-1] |
| printPageCount | int | количество страниц для печати, оно должно быть больше нуля |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Отрендерить рабочую книгу на принтер

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

