---
title: "الفئة LowCodeSaveOptionsProviderOfAssembling"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling. تنفيذ لتوفير خيارات الحفظ التي تحفظ أجزاء مقسمة إلى ملفات ومسار الملف الناتج يُسمّى كما قد يحتوي على أدلة PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

تنفيذ لتوفير خيارات الحفظ التي تحفظ أجزاء مقسمة إلى ملفات ومسار الملف الناتج يُسمّى كما (قد يحتوي على أدلة): [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(or SheetName)+[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | ما إذا كان يتم إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة (أو اسمها) والبادئة المقابلة إلى مسار الملف. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | ما إذا كان يتم إضافة فهرس الجزء المقسم إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء مقسم واحد فقط، لن يتم إضافة فهرس الجزء المقسم والبادئة المقابلة إلى مسار الملف. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | الجزء الرأس (قبل المحتوى المضاف للورقة والجزء المقسم) من مسار الملف. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | الجزء اللاحق (بعد أرقام التسلسل) من مسار الملف. يجب أن يتضمن امتداد اسم الملف. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | القالب لإنشاء مثيل من خيارات الحفظ في [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | بادئة لفهرس ورقة العمل. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | إزاحة فهرس الجزء المقسم بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | بادئة لفهرس الجزء المقسم. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | ما إذا كان يتم بناء مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. القيمة الافتراضية هي false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | يطلق الموارد بعد معالجة الجزء المقسم الحالي. (موروث من [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | يحصل على خيارات الحفظ التي تُستخدم للحصول على إعدادات الإخراج للجزء المقسم الحالي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // تهيئة وتكوين موفر خيارات الحفظ
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // تكوين خيارات حفظ XLSX مع التقسيم باستخدام LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // حفظ المصنف باستخدام الخيارات الممكنة من الموفر باستخدام تنسيق الحفظ الصحيح
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


