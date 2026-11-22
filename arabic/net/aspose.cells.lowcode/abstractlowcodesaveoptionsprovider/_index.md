---
title: "الفئة AbstractLowCodeSaveOptionsProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider. تنفيذ لتوفير خيارات حفظ متعددة للعمليات التي تتطلب مخرجات متعددة. على سبيل المثال، ميزة SpreadsheetSplitter تتطلب وجهات متعددة لحفظ الملفات المقسمة."
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

تنفيذ لتوفير خيارات حفظ متعددة للعمليات التي تتطلب مخرجات متعددة. على سبيل المثال، ميزة [`SpreadsheetSplitter`](../spreadsheetsplitter/) تتطلب وجهات متعددة لحفظ الملفات المقسمة.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | يطلق الموارد بعد معالجة الجزء المقسم الحالي. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | يحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسم الحالي. إرجاع null يعني تخطي الجزء المحدد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // إنشاء موفر مخصص عن طريق توسيع AbstractLowCodeSaveOptionsProvider
            var customProvider = new CustomSaveOptionsProvider();

            // إنشاء مصنف وورقة عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بعض البيانات
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // إنشاء معلومات الجزء المقسم - في الاستخدام الفعلي، ستأتي هذه المعلومات من API
            // نظرًا لعدم إمكانية إنشائه مباشرةً، سنمرر null للتوضيح
            SplitPartInfo splitPartInfo = null;
            
            // الحصول على خيارات الحفظ من الموفر
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // تكوين خيارات الحفظ (مثال)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // إظهار إكمال العملية
            customProvider.Finish(saveOptions);
            
            // حفظ المصنف (ليس له علاقة مباشرة بالموفر، فقط للعرض التجريبي)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // تنفيذ مخصص لـ AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // إنشاء وإرجاع خيارات حفظ مخصصة بناءً على معلومات الجزء
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // تم إزالة CachedFileFolder لأنه غير موجود في LowCodeSaveOptions
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // منطق التنظيف أو الإنهاء هنا
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


