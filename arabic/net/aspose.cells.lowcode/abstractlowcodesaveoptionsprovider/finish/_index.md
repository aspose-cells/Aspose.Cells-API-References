---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractLowCodeSaveOptionsProvider. تُطلق الموارد بعد معالجة الجزء المقسّم حالياً"
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

يطلق الموارد بعد معالجة الجزء المقسم الحالي.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| جزء | LowCodeSaveOptions | خيارات الحفظ المستخدمة للجزء المقسّم حالياً. |

### ملاحظات

بشكل افتراضي، تقوم هذه الطريقة فقط بإغلاق الدفق المحدد بواسطة [`OutputStream`](../../lowcodesaveoptions/outputstream/) مباشرةً (إذا كانت خيارات الحفظ قد حددت Stream كوجهة). يمكن للمستخدم استبدال هذه الطريقة للتحكم في كيفية تحرير الموارد وفقًا لمتطلباته وتنفيذ [`GetSaveOptions`](../getsaveoptions/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // إنشاء كائن مزود ملموس
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // تنفيذ ملموس لـ AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // تنفيذ الطريقة المجردة المطلوبة
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


