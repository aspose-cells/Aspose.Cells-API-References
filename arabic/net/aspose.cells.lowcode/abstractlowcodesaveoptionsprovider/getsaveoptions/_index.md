---
title: "AbstractLowCodeSaveOptionsProvider.GetSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractLowCodeSaveOptionsProvider. تحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسّم حالياً. إرجاع null يعني تخطي الجزء المعطى."
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/
---
## AbstractLowCodeSaveOptionsProvider.GetSaveOptions method

يحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسم الحالي. إرجاع null يعني تخطي الجزء المحدد.

```csharp
public abstract LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // إنشاء كائن مزود ملموس
            var provider = new CustomSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // تنفيذ مخصص لـ AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // إنشاء خيارات حفظ مخصصة بناءً على معلومات الجزء
            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = $"Part_{partInfo.PartIndex}_Sheet_{partInfo.SheetName}.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;

        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


