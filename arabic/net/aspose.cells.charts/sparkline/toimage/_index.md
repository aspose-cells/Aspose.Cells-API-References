---
title: "Sparkline.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Sparkline. تحول sparkline إلى صورة"
type: docs
url: /ar/net/aspose.cells.charts/sparkline/toimage/
---
## ToImage(ImageOrPrintOptions) {#toimage}

يحوّل الـ sparkline إلى صورة.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | ImageOrPrintOptions | خيارات الصورة |

### قيمة الإرجاع

إرجاع كائن Bitmap.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithImageOrPrintOptDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للـ sparkline
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(15);
            sheet.Cells["D1"].PutValue(30);

            // تحديد الموقع للـ sparkline
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            // أضف مجموعة مخطط خطي إلى ورقة العمل.
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];
            Sparkline sparkline = group.Sparklines[0];

            try
            {
                // إنشاء خيارات الصورة بإعدادات واقعية
                ImageOrPrintOptions options = new ImageOrPrintOptions
                {
                    ImageType = Aspose.Cells.Drawing.ImageType.Jpeg,
                    HorizontalResolution = 200,
                    VerticalResolution = 200,
                    Quality = 90,
                    Transparent = false
                };

                // حفظ sparkline إلى ملف باستخدام ToImage مع ImageOrPrintOptions
                sparkline.ToImage("sparkline_demo.jpg", options);

                Console.WriteLine("Sparkline successfully saved as image with custom options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving sparkline as image: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_2}

يحوّل الـ sparkline إلى صورة.

```csharp
public void ToImage(string fileName, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم ملف الصورة. |
| خيارات | ImageOrPrintOptions | خيارات الصورة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SparklineMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            Sparkline line = group.Sparklines[0];

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            line.ToImage("sparkline_output.png", options);
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_1}

يحوّل الـ sparkline إلى صورة.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الصورة. |
| خيارات | ImageOrPrintOptions | خيارات الصورة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineMethodToImageWithStreamImageOrPrintOptDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // حدد CellArea للمخطط الخطي.
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // أضف مجموعة مخطط خطي إلى ورقة العمل.
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            Sparkline line = group.Sparklines[0];

            try
            {
                // إنشاء تدفق ذاكرة لحفظ الصورة
                using (MemoryStream stream = new MemoryStream())
                {
                    // إنشاء خيارات الصورة
                    ImageOrPrintOptions options = new ImageOrPrintOptions
                    {
                        ImageType = Aspose.Cells.Drawing.ImageType.Png,
                        HorizontalResolution = 300,
                        VerticalResolution = 300
                    };

                    // استدعاء طريقة ToImage مع Stream و ImageOrPrintOptions
                    line.ToImage(stream, options);

                    // حفظ التدفق إلى ملف
                    File.WriteAllBytes("sparkline_stream_output.png", stream.ToArray());
                    Console.WriteLine("Sparkline image saved successfully using stream.");
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

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


