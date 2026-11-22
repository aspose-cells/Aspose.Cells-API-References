---
title: "WorkbookRender.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookRender. عرض كامل دفتر العمل كصورة Tiff إلى تدفق"
type: docs
url: /ar/net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

اعرض المصنف بالكامل كصورة Tiff إلى تدفق.

```csharp
public void ToImage(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق الصورة الناتجة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithStreamDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // تكوين خيارات عرض الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // أنشئ دليل الإخراج إذا لم يكن موجودًا
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // إنشاء تدفق ملف لإخراج الصورة
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // تهيئة عارض دفتر العمل وتحويله إلى صورة
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // حفظ دفتر العمل الأصلي للرجوع إليه
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

اعرض المصنف بالكامل كصورة Tiff إلى ملف.

```csharp
public void ToImage(string filename)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الملف | String | اسم ملف الصورة الناتجة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // تعيين خيارات الصورة
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // إنشاء عرض دفتر العمل وحفظه كصورة
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

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
    public class WorkbookRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // إنشاء خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // إنشاء مُصوّر دفتر العمل
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // حفظ كل صفحة كصورة
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

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

    public class WorkbookRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index and Stream Demo";

            // تكوين خيارات عرض الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            try
            {
                // تهيئة عارض دفتر العمل
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // الحصول على فهرس الصفحة الأولى (بدءًا من الصفر)
                int pageIndex = 0;

                // إنشاء تدفق ذاكرة لاحتواء الصورة
                using (MemoryStream stream = new MemoryStream())
                {
                    // استدعاء ToImage مع فهرس الصفحة والتدفق
                    renderer.ToImage(pageIndex, stream);

                    // عرض النتائج
                    Console.WriteLine($"Page {pageIndex} rendered successfully to stream");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");
                    Console.WriteLine($"Total pages available: {renderer.PageCount}");
                }
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

* class [WorkbookRender](../)
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
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index Demo";

            // تكوين خيارات عرض الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

            // أنشئ دليل الإخراج إذا لم يكن موجودًا
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            try
            {
                // تهيئة عارض دفتر العمل
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // الحصول على فهرس الصفحة الأولى (بدءًا من الصفر)
                int pageIndex = 0;

                // استدعاء ToImage مع فهرس الصفحة وحفظه إلى ملف
                string imagePath = Path.Combine(outputDir, $"page_{pageIndex}.png");
                renderer.ToImage(pageIndex, imagePath);

                Console.WriteLine($"Page {pageIndex} rendered successfully to: {imagePath}");
                Console.WriteLine($"Total pages available: {renderer.PageCount}");
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

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


