---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ImageOrPrintOptions. تحدد العرض والارتفاع المطلوبين للصورة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

يضبط العرض والارتفاع المطلوبين للصورة.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| desiredWidth | Int32 | العرض المطلوب بالبكسل |
| desiredHeight | Int32 | الارتفاع المطلوب بالبكسل |

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام `SetDesiredSize` عن طريق تعيين المعامل keepAspectRatio إلى false. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2023. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // تعيين منطقة الطباعة
            worksheet.PageSetup.PrintArea = "A1:A11";

            // إنشاء خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // تحويل ورقة العمل إلى صورة
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

يضبط العرض والارتفاع المطلوبين للصورة.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| desiredWidth | Int32 | العرض المطلوب بالبكسل |
| desiredHeight | Int32 | الارتفاع المطلوب بالبكسل |
| keepAspectRatio | منطقي | ما إذا كان يجب الحفاظ على نسبة أبعاد الصورة الأصلية |

### ملاحظات

سيعتمد عرض وارتفاع الصورة الناتجة بالبكسل فقط على العرض والارتفاع المطلوبين المحددين.

لن تؤثر [`HorizontalResolution`](../horizontalresolution/) و[`VerticalResolution`](../verticalresolution/) على عرض وارتفاع الصورة الناتجة في هذه الحالة.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
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

            // احصل على شكل المخطط
            Shape chartShape = worksheet.Shapes[0];

            // تعيين خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // احفظ المخطط كصورة
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // احفظ الصورة إلى ملف
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


