---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeImageSaveOptions. موفر خيارات الحفظ لحفظ الصور المُولَّدة"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

موفر خيارات الحفظ لحفظ الصور المولدة.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### ملاحظات

المخرجات([`OutputFile`](../../lowcodesaveoptions/outputfile/) أو [`OutputStream`](../../lowcodesaveoptions/outputstream/)) المحددة بواسطة هذه الحالة لن يكون لها أي تأثير عندما يتم تحديد هذه الخاصية. بدلاً من ذلك، سيتم تحديد مخرجات كل صورة مُولَّدة بواسطة الموفر.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // إنشاء كائن LowCodeImageSaveOptions
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // إنشاء SaveOptionsProvider مخصص
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // عرض موفر SaveOptionsProvider الحالي
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // إظهار التأثير عن طريق الحفظ باستخدام خيارات مختلفة
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // تغيير إلى موفر فارغ
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // إرجاع خيارات حفظ مخصصة لكل جزء
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // إجراء أي تنظيف بعد الحفظ
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


