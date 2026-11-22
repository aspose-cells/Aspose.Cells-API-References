---
title: "الفئة LowCodeImageSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LowCode.LowCodeImageSaveOptions. خيارات حفظ الصورة بطريقة منخفضة الكود"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

خيارات حفظ الصورة بطريقة منخفضة الكود.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | الخيارات الخاصة بتصيير الصور. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | الحصول وتعيين الملف (مع المسار إذا لزم) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [`OutputStream`](../lowcodesaveoptions/outputstream/). (موروث من [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | الحصول وتعيين الدفق لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل [`OutputFile`](../lowcodesaveoptions/outputfile/). (موروث من [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | يحصل أو يحدد تنسيق الحفظ. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | موفر خيارات الحفظ لحفظ الصور المولدة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة بيانات عينة إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // إنشاء نسخة من LowCodeImageSaveOptions
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // تعيين الخصائص الأساسية
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // عرض الإعدادات الحالية
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // تعديل بعض خيارات الصورة
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // إنشاء موفر خيارات حفظ بسيط
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // حفظ ورقة العمل كصورة
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


