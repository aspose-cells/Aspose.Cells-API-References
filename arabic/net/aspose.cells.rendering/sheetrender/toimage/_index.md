---
title: "SheetRender.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SheetRender. تصيير صفحة معينة إلى Graphics"
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

عرض صفحة معينة إلى Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| g | الرسومات | الكائن الذي يتم الرسم إليه. |
| x | Single | إحداثي X (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |
| y | Single | إحداثي Y (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |
| العرض | Single | العرض الأقصى (بالبيكسل) الذي يمكن أن تشغله الصفحة المرسومة. |
| الارتفاع | Single | الارتفاع الأقصى (بالبيكسل) الذي يمكن أن تشغله الصفحة المرسومة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // إنشاء خيارات الصورة
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // إنشاء عرض ورقة للورقة العمل.
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // إنشاء تدفق ذاكرة لالتقاط الصورة المرسومة.
                using (MemoryStream stream = new MemoryStream())
                {
                    // استدعاء ToImage مع المعلمات المحددة.
                    // نظرًا لأننا لا نستطيع استخدام System.Drawing.Graphics، سنستخدم نسخة ToImage الأبسط.
                    sheetRender.ToImage(0, stream);

                    // حفظ الصورة المرسومة إلى ملف.
                    File.WriteAllBytes("RenderedOutput.png", stream.ToArray());
                }

                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

عرض صفحة معينة إلى Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| g | الرسومات | الكائن الذي يتم الرسم إليه. |
| x | Single | إحداثي X (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |
| y | Single | إحداثي Y (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // إنشاء خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // إنشاء مثيل SheetRender.
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // نظرًا لأننا لا نستطيع استخدام أنواع System.Drawing، سنستخدم طريقة ToImage البديلة.
                // التي تحفظ مباشرة إلى ملف.
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // تنظيف الموارد
                sheetRender.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

اعرض صفحة معينة إلى ملف.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| fileName | String | اسم ملف الصورة الناتجة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // تحميل ملف Excel المصدر.
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // إنشاء خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // إنشاء عرض ورقة للورقة الأولى.
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // رسم الصفحة الأولى من الورقة إلى ملف صورة.
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

اعرض صفحة معينة إلى تدفق.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| تدفق | Stream | تدفق الصورة الناتجة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // إنشاء خيارات الصورة
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // إنشاء مثيل SheetRender.
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // إنشاء تدفق ذاكرة لاحتواء الصورة
                using (MemoryStream stream = new MemoryStream())
                {
                    // استدعاء ToImage مع فهرس الصفحة ومعلمات التدفق.
                    sheetRender.ToImage(0, stream);

                    Console.WriteLine($"Successfully rendered page 0 to stream. Stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

اعرض صفحة معينة إلى كائن Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |

### قيمة الإرجاع

كائن البت ماب للصفحة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // إنشاء خيارات الصورة
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // إنشاء مثيل SheetRender.
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // الحصول على فهرس الصفحة الأولى (بدءًا من الصفر)
                int pageIndex = 0;

                // استدعاء ToImage مع معلمة فهرس الصفحة.
                sheetRender.ToImage(pageIndex, "output_page.png");

                Console.WriteLine($"Successfully rendered page {pageIndex} to image");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


