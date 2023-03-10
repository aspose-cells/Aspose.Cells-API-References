---
title: طريقة to_image
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 120
url: /ar/python-net/aspose.cells.charts/chart/to_image/
is_root: false
---
##  to_image(image_file) {#str}
ينشئ صورة المخطط ويحفظها في ملف.
يحدد امتداد اسم الملف تنسيق الصورة.



```python
def to_image(self, image_file):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| image_file | str | اسم ملف الصورة بالمسار الكامل.|
###  ملاحظات

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف.
على سبيل المثال ، إذا حددت "myfile.png" ، فسيتم حفظ الصورة
 بتنسيق PNG. يتم التعرف على امتدادات الملفات التالية:
.bmp ، .gif ، .png ، .jpg ، .jpeg ، .tiff ، .tif ، .emf.


إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا.

##  to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}
ينشئ صورة المخطط ويحفظها في ملف في نوع الصورة المحدد.



```python
def to_image(self, image_file, image_type):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| image_file | str | اسم ملف الصورة بالمسار الكامل.|
| image_type | aspose.cells.drawing.ImageType | نوع الصورة المراد حفظ الصورة بها.|
###  ملاحظات

تم تحديد نوع الصورة باستخدام `imageType`.
 الأنواع التالية مدعومة:
ImageType.Bmp و ImageType.Gif و ImageType.Png و ImageType.Jpeg و ImageType.Tiff و ImageType.Emf.


إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا.

##  to_image(image_file, jpeg_quality) {#str-int}
ينشئ صورة المخطط ويحفظها في ملف بتنسيق Jpeg.



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| image_file | str | اسم ملف الصورة بالمسار الكامل.|
| jpeg_quality | int | جودة JPEG.|
###  ملاحظات

إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا.

##  to_image(stream, jpeg_quality) {#io.RawIOBase-int}

ينشئ صورة المخطط ويحفظها في دفق بتنسيق Jpeg.



```python
def to_image(self, stream, jpeg_quality):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | تيار الإخراج.|
| jpeg_quality | int | جودة JPEG.|
###  ملاحظات

إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا.

##  to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

ينشئ صورة المخطط ويحفظها في دفق بالتنسيق المحدد.



```python
def to_image(self, stream, image_type):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | تيار الإخراج.|
| image_type | aspose.cells.drawing.ImageType | نوع الصورة المراد حفظ الصورة بها.|
###  ملاحظات

تم تحديد نوع الصورة باستخدام `imageType`.
 الأنواع التالية مدعومة:
ImageType.Bmp و ImageType.Gif و ImageType.Png و ImageType.Jpeg و ImageType.Tiff و ImageType.Emf.


إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا.

##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
ينشئ صورة المخطط ويحفظها في ملف.
يحدد امتداد اسم الملف تنسيق الصورة.



```python
def to_image(self, image_file, options):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| image_file | str | اسم ملف الصورة بالمسار الكامل.|
| options | aspose.cells.rendering.ImageOrPrintOptions | خيارات إنشاء الصور الإضافية|
###  ملاحظات

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف.
على سبيل المثال ، إذا حددت "myfile.png" ، فسيتم حفظ الصورة
 بتنسيق PNG. يتم التعرف على امتدادات الملفات التالية:
.bmp ، .gif ، .png ، .jpg ، .jpeg ، .tiff ، .tif ، .emf.


إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا.
 يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)لمزيد من التفاصيل.
###  مثال

يحفظ في Tiff بدقة 300 نقطة في البوصة وضغط CCITT4.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, TiffCompression

options = ImageOrPrintOptions()
options.horizontal_resolution = 300
options.vertical_resolution = 300
options.tiff_compression = TiffCompression.COMPRESSION_CCITT4
book = Workbook(r"test.xls")
book.worksheets[0].charts[0].to_image(r"chart.Tiff", options)

```


يحفظ في Jpeg بدقة 300 نقطة في البوصة وجودة صورة 80.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions

options = ImageOrPrintOptions()
options.horizontal_resolution = 300
options.vertical_resolution = 300
options.quality = 80
book = Workbook(r"test.xls")
book.worksheets[0].charts[0].to_image(r"chart.Jpeg", options)

```


##  to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
ينشئ صورة المخطط ويحفظها في دفق بالتنسيق المحدد.



```python
def to_image(self, stream, options):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | تيار الإخراج.|
| options | aspose.cells.rendering.ImageOrPrintOptions | خيارات إنشاء الصور الإضافية|
###  ملاحظات

تم تحديد نوع الصورة باستخدام `options.ImageType`.
 التنسيقات التالية مدعومة:
ImageType.Bmp و ImageType.Gif و ImageType.Png و ImageType.Jpeg و ImageType.Tiff و ImageType.Emf.


إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا.
 يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)لمزيد من التفاصيل.


###  أنظر أيضا
* وحدة [aspose.cells.charts](../../)
* فئة [Chart](/cells/ar/python-net/aspose.cells.charts/chart)
