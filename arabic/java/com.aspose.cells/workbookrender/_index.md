---
title: "WorkbookRender"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عرضًا للمصنف."
type: docs
url: /ar/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

يمثل عرض Workbook. يجب استخدام منشئ هذه الفئة بعد تعديل pagesetup، cell style.

**Remarks**
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | إنشاء WorkbookRender |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [dispose()](#dispose--) | يطلق الموارد التي تم إنشاؤها واستخدامها في العرض. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | يحصل على العدد الإجمالي للصفحات في workbook. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | احصل على حجم الصفحة بالبوصة للصورة الناتجة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | عرض صفحة معينة إلى تدفق. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | عرض صفحة معينة إلى تدفق. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | عرض صفحة معينة إلى ملف. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | عرض كامل workbook كصورة Tiff إلى تدفق. |
| [toImage(String filename)](#toImage-java.lang.String-) | عرض كامل workbook كصورة Tiff إلى ملف. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | عرض workbook إلى الطابعة |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | عرض workbook إلى الطابعة |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | عرض workbook إلى الطابعة |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


إنشاء WorkbookRender

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | حدد أي workbook سيتم عرضه. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions يحتوي على بعض خصائص الصورة الناتجة |

### dispose() {#dispose--}
```
public void dispose()
```


يطلق الموارد التي تم إنشاؤها واستخدامها في العرض.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحصل على العدد الإجمالي للصفحات في workbook.

**Returns:**
int
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


احصل على حجم الصفحة بالبوصة للصورة الناتجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageIndex | int | مؤشر الصفحة يبدأ من الصفر. |

**Returns:**
float[] - حجم صورة الصفحة، [0] للعرض و[1] للارتفاع
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


عرض صفحة معينة إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageIndex | int | حدد أي صفحة سيتم تحويلها |
| stream | java.io.InputStream | تدفق الصورة الناتجة |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


عرض صفحة معينة إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageIndex | int | حدد أي صفحة سيتم تحويلها |
| stream | java.io.OutputStream | تدفق الصورة الناتجة |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


عرض صفحة معينة إلى ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageIndex | int | حدد أي صفحة سيتم تحويلها |
| fileName | java.lang.String | اسم ملف الصورة الناتجة |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


عرض كامل workbook كصورة Tiff إلى تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.OutputStream | تدفق الصورة الناتجة |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


عرض كامل workbook كصورة Tiff إلى ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الملف | java.lang.String | اسم ملف الصورة الناتجة |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


عرض workbook إلى الطابعة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


عرض workbook إلى الطابعة

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام ToPrinter(string PrinterName) و ImageOrPrintOptions.PageIndex, PageCount لتعيين الصفحة الأولى وعدد الصفحات للطباعة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2021. Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer" |
| printPageIndex | int | الفهرس القائم على الصفر للصفحة الأولى للطباعة، يجب أن يكون ضمن النطاق [0, WorkbookRender.PageCount-1] |
| printPageCount | int | عدد الصفحات للطباعة، يجب أن يكون أكبر من الصفر |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


عرض workbook إلى الطابعة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | تعيين اسم مهمة الطباعة |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

