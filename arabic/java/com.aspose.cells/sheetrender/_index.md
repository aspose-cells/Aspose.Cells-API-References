---
title: "SheetRender"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عرض ورقة عمل يمكنه تحويل ورقة العمل إلى صور مختلفة مثل BMP PNG JPEG TIFF.."
type: docs
url: /ar/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

يمثل عرض ورقة عمل يمكنه تحويل ورقة العمل إلى صور مختلفة مثل (BMP, PNG, JPEG, TIFF..) يجب استخدام منشئ هذه الفئة بعد تعديل إعدادات الصفحة، نمط الخلية.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | إنشاء SheetRender يحتاج إلى ورقة عمل و ImageOrPrintOptions كمعاملات |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [dispose()](#dispose--) | يطلق الموارد التي تم إنشاؤها واستخدامها في العرض. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | يحصل على العدد الإجمالي للصفحات في ورقة العمل الحالية. |
| [getPageScale()](#getPageScale--) | يحصل على مقياس الصفحة المحسوب للورقة. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | احصل على حجم الصفحة بالبوصة للصورة الناتجة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | عرض صفحة معينة إلى تدفق. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | عرض صفحة معينة إلى تدفق. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | عرض صفحة معينة إلى ملف. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | عرض ورقة العمل إلى الطابعة |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | عرض ورقة العمل إلى الطابعة |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | عرض ورقة العمل إلى الطابعة |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | عرض كامل ورقة العمل كصورة Tiff إلى التدفق. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


إنشاء SheetRender يحتاج إلى ورقة عمل و ImageOrPrintOptions كمعاملات

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | حدد أي جدول بيانات سيتم عرضه. |
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


يحصل على العدد الإجمالي للصفحات في ورقة العمل الحالية.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


يحصل على مقياس الصفحة المحسوب للورقة. يرجع المقياس المحدد إذا تم تعيين [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) . وإلا، يرجع المقياس المحسوب وفقًا لـ [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) و [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--).

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

**Example**

الكود التالي يخرج الصفحة الأولى من الورقة الأولى إلى صورة png.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageIndex | int | حدد أي صفحة سيتم تحويلها |
| fileName | java.lang.String | اسم ملف الصورة الناتجة |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


عرض ورقة العمل إلى الطابعة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


عرض ورقة العمل إلى الطابعة

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام ToPrinter(string PrinterName) و ImageOrPrintOptions.PageIndex, PageCount لتعيين الصفحة الأولى وعدد الصفحات للطباعة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2021. Aspose تعتذر عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer" |
| printPageIndex | int | الفهرس القائم على الصفر للصفحة الأولى للطباعة، يجب أن يكون في النطاق [0, SheetRender.PageCount-1] |
| printPageCount | int | عدد الصفحات للطباعة، يجب أن يكون أكبر من الصفر |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


عرض ورقة العمل إلى الطابعة

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
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


عرض كامل ورقة العمل كصورة Tiff إلى التدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | تدفق الصورة الناتجة |

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

