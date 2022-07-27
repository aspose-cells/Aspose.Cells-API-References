---
title: ToImage
second_title: Aspose.Cells لمرجع .NET API
description: يحصل على 32 بتنقطية كائن من الرسم البياني .
type: docs
weight: 590
url: /ar/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

يحصل على 32 بت`نقطية` كائن من الرسم البياني .

```csharp
public Bitmap ToImage()
```

### قيمة الإرجاع

صورة الرسم البياني.

### ملاحظات

إذا كان العرض أو الارتفاع صفراً أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فسيعود فارغًا. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أنظر أيضا

* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

يحصل على 32 بت`نقطية` كائن من الرسم البياني . `خيارات ImageOrPrintOptions. تنسيق الصورة` و ImageOrPrintOptions.TiffCompression و ImageOrPrintOptions. يتم تجاهل سمات الجودة.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| options | ImageOrPrintOptions | خيارات إنشاء الصور الإضافية |

### قيمة الإرجاع

صورة الرسم البياني.

### ملاحظات

لا تؤثر سمات ImageOrPrintOptions.ImageFormat و ImageOrPrintOptions.TiffCompression و ImageOrPrintOptions.Quality على الطريقة. سيعود فارغة. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أمثلة

الحصول على كائن نقطي بدقة 200 × نقطة في البوصة و 300 نقطة في البوصة.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 200;
options.VerticalResolution = 300;

Workbook book = new Workbook(@"test.xls");
Bitmap chartObject = book.Worksheets[0].Charts[0].ToImage(options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 200
options.VerticalResolution = 300

Dim book As Workbook =  New Workbook("test.xls")
Dim chartObject As Bitmap = book.Worksheets(0).Charts(0).ToImage(options)

```

### أنظر أيضا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة.

```csharp
public void ToImage(string imageFile)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة بالمسار الكامل. |

### ملاحظات

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف . على سبيل المثال ، إذا حددت "myfile.png" ، فسيتم حفظ الصورة بتنسيق PNG. يتم التعرف على امتدادات الملفات التالية: .bmp ، .gif ، .png ، .jpg ، .jpeg ، .tiff ، .tif ، .emf.

إذا كان العرض أو الارتفاع صفرًا أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أنظر أيضا

* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

لإنشاء صورة الرسم البياني وحفظها في ملف من نوع الصورة المحدد.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة بالمسار الكامل. |
| imageType | ImageType | نوع الصورة المراد حفظ الصورة بها. |

### ملاحظات

يتم تحديد نوع الصورة باستخدام`نوع الصورة`. الأنواع التالية مدعومة: ImageType.Bmp و ImageType.Gif و ImageType.Png و ImageType.Jpeg و ImageType.Tiff و ImageType.Emf.

إذا كان العرض أو الارتفاع صفرًا أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أنظر أيضا

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

لإنشاء صورة المخطط وحفظها في ملف بتنسيق Jpeg .

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة بالمسار الكامل. |
| jpegQuality | Int64 | جودة JPEG. |

### ملاحظات

إذا كان العرض أو الارتفاع صفرًا أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أنظر أيضا

* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

لإنشاء صورة المخطط وحفظها في تدفق بتنسيق Jpeg .

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | تيار الإخراج. |
| jpegQuality | Int64 | جودة JPEG. |

### ملاحظات

إذا كان العرض أو الارتفاع صفرًا أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أنظر أيضا

* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

لإنشاء صورة المخطط وحفظها في دفق بالتنسيق المحدد.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | تيار الإخراج. |
| imageType | ImageType | نوع الصورة المراد حفظ الصورة بها. |

### ملاحظات

يتم تحديد نوع الصورة باستخدام`نوع الصورة`. الأنواع التالية مدعومة: ImageType.Bmp و ImageType.Gif و ImageType.Png و ImageType.Jpeg و ImageType.Tiff و ImageType.Emf.

إذا كان العرض أو الارتفاع صفرًا أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا . يرجى الرجوع[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أنظر أيضا

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة بالمسار الكامل. |
| options | ImageOrPrintOptions | خيارات إنشاء الصور الإضافية |

### ملاحظات

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف . على سبيل المثال ، إذا حددت "myfile.png" ، فسيتم حفظ الصورة بتنسيق PNG. يتم التعرف على امتدادات الملفات التالية: .bmp ، .gif ، .png ، .jpg ، .jpeg ، .tiff ، .tif ، .emf.

إذا كان العرض أو الارتفاع صفرًا أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أمثلة

يحفظ في Tiff بدقة 300 نقطة في البوصة وضغط CCITT4. يحفظ في Jpeg بدقة 300 نقطة في البوصة وجودة صورة 80.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.TiffCompression = TiffCompression.CompressionCCITT4;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Tiff", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.TiffCompression = TiffCompression.CompressionCCITT4

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Tiff", options)

```

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.Quality = 80;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Jpeg", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions()
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.Quality = 80

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Jpeg", options)

```

### أنظر أيضا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

لإنشاء صورة المخطط وحفظها في دفق بالتنسيق المحدد.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| stream | Stream | تيار الإخراج. |
| options | ImageOrPrintOptions | خيارات إنشاء الصور الإضافية |

### ملاحظات

يتم تحديد نوع الصورة باستخدام`خيارات`. التنسيقات التالية مدعومة: ImageType.Bmp و ImageType.Gif و ImageType.Png و ImageType.Jpeg و ImageType.Tiff و ImageType.Emf.

إذا كان العرض أو الارتفاع صفرًا أو كان الرسم البياني غير مدعوم وفقًا لقائمة الرسوم البيانية المدعومة ، فلن تفعل هذه الطريقة شيئًا. يرجى الرجوع إلى[قائمة الرسوم البيانية المدعومة](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أنظر أيضا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* مساحة الاسم [Aspose.Cells.Charts](../../chart)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
