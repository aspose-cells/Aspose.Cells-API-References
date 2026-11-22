---
title: "LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LowCodeSaveOptionsProviderOfAssembling. تحصل على خيارات الحفظ التي تُستَخدم للحصول على إعدادات الإخراج للجزء المقسم حاليًا"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method

يحصل على خيارات الحفظ التي تُستخدم للحصول على إعدادات الإخراج للجزء المقسم الحالي.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].Value = "Sample Data for Split";

            try
            {
                // إنشاء نسخة من LowCodeSaveOptionsProviderOfAssembling
                var provider = new LowCodeSaveOptionsProviderOfAssembling
                {
                    PathHeader = "Output/",
                    PathTail = ".xlsx",
                    UseSheetName = true,
                    SheetPrefix = "Sheet_",
                    SplitPartPrefix = "Part_",
                    SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
                };

                // إنشاء كائن SplitPartInfo باستخدام الانعكاس لأن المُنشئ غير قابل للوصول
                var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);

                // استدعاء GetSaveOptions مع معامل SplitPartInfo
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                Console.WriteLine("SaveOptions created successfully");
                Console.WriteLine($"Output format: {saveOptions.SaveFormat}");

                // احفظ دفتر العمل (في الاستخدام الفعلي سيستخدم خيارات الحفظ المُولدة)
                workbook.Save("GetSaveOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


