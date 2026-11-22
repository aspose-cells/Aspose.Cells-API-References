---
title: "الفئة LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders. تنفيذ لتوفير خيارات الحفظ التي تحفظ أجزاء مقسمة إلى ملفات ومسار الملف الناتج يُحدَّد باستخدام العناصر النائبة"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

تنفيذ لتوفير خيارات حفظ تقوم بحفظ الأجزاء المقسمة إلى ملفات وتُعرّف مسارات الملفات الناتجة باستخدام عناصر نائبة.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | ينشئ نسخة لتوفير خيارات الحفظ وفقًا للقوالب المحددة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | ما إذا كان يجب إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة والاسم والبادئة المقابلة ([`SheetNamePrefix`](./sheetnameprefix/)) إلى مسار الملف. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | ما إذا كان يجب إضافة فهرس جزء الانقسام إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء انقسام واحد فقط، لن يتم إضافة فهرس جزء الانقسام والبادئة المقابلة ([`SplitPartPrefix`](./splitpartprefix/)) إلى مسار الملف. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | القالب لإنشاء مثيل من خيارات الحفظ في [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | بادئة لفهرس ورقة العمل. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | بادئة لفهرس ورقة العمل. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | إزاحة فهرس الجزء المقسم بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | بادئة لفهرس الجزء المقسم. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | يطلق الموارد بعد معالجة الجزء المقسم الحالي. (موروث من [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | يحصل على خيارات الحفظ التي تُستخدم للحصول على إعدادات الإخراج للجزء المقسم الحالي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء ورقة العمل ببيانات نموذجية
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // إنشاء موفر باستخدام قالب مسار يحتوي على عناصر نائبة
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // تكوين خصائص الموفر
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // تكوين قالب خيارات الحفظ
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // تكوين خيارات الصورة أو الطباعة للتصوير المقسّم
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // إنشاء عرض ورقة مع تكوين التقسيم
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


