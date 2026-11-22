---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ ImageSaveOptions. ينشئ الخيارات لحفظ ملف الصورة"
type: docs
url: /ar/net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

ينشئ الخيارات لحفظ ملف الصورة.

```csharp
public ImageSaveOptions()
```

### ملاحظات

النوع الافتراضي هو Tiff.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ImageSaveOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // عرض مثال على المنشئ بدون معلمات
                ImageSaveOptions defaultOptions = new ImageSaveOptions();
                Console.WriteLine("Created ImageSaveOptions with default constructor");

                // عرض مثال على المنشئ مع معامل SaveFormat
                ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
                Console.WriteLine("Created ImageSaveOptions with SaveFormat.Png");

                // الوصول إلى خاصية ImageOrPrintOptions للقراءة فقط
                var imageOptions = pngOptions.ImageOrPrintOptions;
                Console.WriteLine($"ImageOrPrintOptions type: {imageOptions.GetType().Name}");

                // تعيين خاصية StreamProvider
                pngOptions.StreamProvider = null;
                Console.WriteLine("StreamProvider set to null");

                // حفظ المصنف باستخدام الخيارات التي تم إنشاؤها
                workbook.Save("output.png", pngOptions);
                Console.WriteLine("Workbook saved successfully with ImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

ينشئ الخيارات لحفظ ملف الصورة.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | SaveFormat | تنسيق الملف. يجب أن يكون أحد الأنواع التالية: Tiff، Svg، Bmp، Png، Jpg، Emf أو Gif، وإلا سيتم تعيين تنسيق الحفظ تلقائيًا إلى Tiff. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد وإضافة بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
            
            // إنشاء ImageSaveOptions مع SaveFormat.Tiff
            try
            {
                ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
                
                // تكوين خيارات عرض الصورة
                saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
                saveOptions.ImageOrPrintOptions.VerticalResolution = 300;

                // حفظ دفتر العمل كملف TIFF متعدد الصفحات
                workbook.Save("WorksheetImage.tiff", saveOptions);
                
                Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image save operation: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


