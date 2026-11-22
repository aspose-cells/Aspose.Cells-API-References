---
title: "Chart.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Chart. تحصل على كائن Bitmap 32 بت للمخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

يحصل على كائن `Bitmap` 32-بت للمخطط.

```csharp
public Bitmap ToImage()
```

### قيمة الإرجاع

صورة المخطط.

### ملاحظات

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فسيعيد null.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);
            
            // تحويل المخطط إلى صورة وحفظه في ملف
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

يحصل على كائن `Bitmap` 32-بت للمخطط. يتم تجاهل سمات `ImageOrPrintOptions.ImageFormat`، ImageOrPrintOptions.TiffCompression و ImageOrPrintOptions.Quality.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | ImageOrPrintOptions | خيارات إضافية لإنشاء الصورة |

### قيمة الإرجاع

صورة المخطط.

### ملاحظات

يعيد كائن bitmap 32 بت، لذا فإن خصائص ImageOrPrintOptions.ImageFormat و ImageOrPrintOptions.TiffCompression و ImageOrPrintOptions.Quality لا تؤثر على الطريقة. إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فسيعيد null.

### أمثلة

يحصل على كائن bitmap بدقة 200 نقطة في البوصة على المحور x و 300 نقطة في البوصة على المحور y.

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

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة.

```csharp
public void ToImage(string imageFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة مع المسار الكامل. |

### ملاحظات

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف. على سبيل المثال، إذا حددت "myfile.png"، فسيتم حفظ الصورة بتنسيق PNG. يتم التعرف على امتدادات الملفات التالية: .bmp، .gif، .png، .jpg، .jpeg، .tiff، .tif، .emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فلن تقوم هذه الطريقة بأي شيء.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // حفظ المخطط كصورة
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

ينشئ صورة المخطط ويحفظها في ملف بالتنسيق المحدد.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة مع المسار الكامل. |
| imageFormat | ImageFormat | التنسيق الذي سيتم حفظ الصورة به. |

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة Chart.ToImage(string, ImageType). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

ينشئ صورة المخطط ويحفظها في ملف بنوع الصورة المحدد.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة مع المسار الكامل. |
| imageType | ImageType | نوع الصورة الذي سيتم حفظها به. |

### ملاحظات

يتم تحديد نوع الصورة باستخدام `imageType`. الأنواع التالية مدعومة: ImageType.Bmp، ImageType.Gif، ImageType.Png، ImageType.Jpeg، ImageType.Tiff، ImageType.Emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فلن تقوم هذه الطريقة بأي شيء.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // حفظ المخطط كصورة باستخدام ImageType المحدد
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

ينشئ صورة المخطط ويحفظها في ملف بصيغة Jpeg.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة مع المسار الكامل. |
| jpegQuality | Int64 | جودة Jpeg. |

### ملاحظات

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تفعل شيئًا. ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة ToImage(string,ImageOrPrintOptions) مع الجودة المحددة. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ مارس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodToImageWithStringInt64Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // استدعِ طريقة ToImage مع المعلمات (String, Int64)
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

ينشئ صورة المخطط ويحفظها في تدفق بتنسيق Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الإخراج. |
| jpegQuality | Int64 | جودة Jpeg. |

### ملاحظات

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فلن تقوم هذه الطريقة بأي شيء.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamInt64Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // إنشاء تدفق ذاكرة لحفظ الصورة
                using (MemoryStream stream = new MemoryStream())
                {
                    // استدعِ طريقة ToImage مع معلمات Stream و Int64
                    // تم تحديد جودة JPEG كـ 80 (النطاق الصالح عادةً من 0 إلى 100)
                    chart.ToImage(stream, 80);

                    // عرض رسالة النجاح
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // احفظ المصنف
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

ينشئ صورة المخطط ويحفظها في تدفق بالتنسيق المحدد.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الإخراج. |
| imageFormat | ImageFormat | التنسيق الذي سيتم حفظ الصورة به. |

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام طريقة Chart.ToImage(Stream, ImageType). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // إنشاء تدفق ذاكرة لحفظ الصورة
                using (MemoryStream stream = new MemoryStream())
                {
                    // استدعِ طريقة ToImage مع معلمات Stream و ImageFormat
                    // استخدام Aspose.Cells.Drawing.ImageType بدلاً من System.Drawing.Imaging.ImageFormat
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // عرض رسالة النجاح
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // اختياريًا، احفظ الدفق في ملف للتحقق.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToImage: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

ينشئ صورة المخطط ويحفظها في تدفق بالتنسيق المحدد.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الإخراج. |
| imageType | ImageType | نوع الصورة الذي سيتم حفظها به. |

### ملاحظات

يتم تحديد نوع الصورة باستخدام `imageType`. الأنواع التالية مدعومة: ImageType.Bmp، ImageType.Gif، ImageType.Png، ImageType.Jpeg، ImageType.Tiff، ImageType.Emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فلن تقوم هذه الطريقة بأي شيء.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // إنشاء تدفق ذاكرة لحفظ الصورة
                using (MemoryStream stream = new MemoryStream())
                {
                    // استدعِ طريقة ToImage مع معلمات Stream و ImageType
                    chart.ToImage(stream, ImageType.Png);

                    // عرض رسالة النجاح
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // احفظ الصورة في ملف للتوضيح.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // احفظ المصنف
                workbook.Save("ChartToImageDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFile | String | اسم ملف الصورة مع المسار الكامل. |
| خيارات | ImageOrPrintOptions | خيارات إضافية لإنشاء الصورة |

### ملاحظات

يتم تحديد تنسيق الصورة باستخدام امتداد اسم الملف. على سبيل المثال، إذا حددت "myfile.png"، فسيتم حفظ الصورة بتنسيق PNG. يتم التعرف على امتدادات الملفات التالية: .bmp، .gif، .png، .jpg، .jpeg، .tiff، .tif، .emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تفعل شيئًا. يرجى الرجوع إلى [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // إنشاء خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // حمّل المصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة وأنشئ مخططًا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // احفظ المخطط كصورة
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

ينشئ صورة المخطط ويحفظها في تدفق بالتنسيق المحدد.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الإخراج. |
| خيارات | ImageOrPrintOptions | خيارات إضافية لإنشاء الصورة |

### ملاحظات

يتم تحديد نوع الصورة باستخدام `options.ImageType`. الصيغ التالية مدعومة: ImageType.Bmp، ImageType.Gif، ImageType.Png، ImageType.Jpeg، ImageType.Tiff، ImageType.Emf.

إذا كان العرض أو الارتفاع صفرًا أو لم يكن المخطط مدعومًا وفقًا لقائمة المخططات المدعومة، فإن هذه الطريقة لن تفعل شيئًا. يرجى الرجوع إلى [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) لمزيد من التفاصيل.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageOrPrintOptDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // إنشاء تدفق ذاكرة لحفظ الصورة
                using (MemoryStream stream = new MemoryStream())
                {
                    // إنشاء ImageOrPrintOptions بإعدادات محددة
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // استدعِ طريقة ToImage مع معلمات Stream و ImageOrPrintOptions
                    chart.ToImage(stream, options);

                    // عرض رسالة النجاح
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // احفظ المصنف
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


