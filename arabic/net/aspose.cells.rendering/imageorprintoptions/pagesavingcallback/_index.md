---
title: "ImageOrPrintOptions.PageSavingCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. التحكم/الإشارة إلى تقدم عملية حفظ الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/pagesavingcallback/
---
## ImageOrPrintOptions.PageSavingCallback property

التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وتعبئة البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات تجريبية تمتد عبر صفحات متعددة
            worksheet.Cells["A1"].PutValue("PageSavingCallback Demonstration");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Data Row {i}");
            }

            // تكوين إعداد الصفحة لإنشاء صفحات متعددة
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Orientation = PageOrientationType.Portrait;
            pageSetup.FitToPagesWide = 1;
            pageSetup.FitToPagesTall = 0;

            // تهيئة ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4
            };

            // عرض حالة الاستدعاء الأولية
            Console.WriteLine($"Initial PageSavingCallback: {options.PageSavingCallback}");

            // تعيين استدعاء حفظ الصفحة المخصص
            options.PageSavingCallback = new CustomPageSavingCallback();

            // تصيير ورقة العمل إلى TIFF متعدد الصفحات
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("output_with_callback.tiff");

            // احفظ المصنف للرجوع إليه
            workbook.Save("PageSavingCallbackDemo.xlsx");
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Processing page {args.PageIndex}");
                
                // تخطي الصفحة الأولى (فهرس يبدأ من الصفر)
                if (args.PageIndex == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine("Skipping first page");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                Console.WriteLine($"Completed processing page {args.PageIndex}");
            }
        }
    }
}
```

### انظر أيضًا

* interface [IPageSavingCallback](../../ipagesavingcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


