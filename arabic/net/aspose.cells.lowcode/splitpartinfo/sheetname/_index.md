---
title: "SplitPartInfo.SheetName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SplitPartInfo. اسم الورقة التي يوجد فيها الجزء الحالي"
type: docs
url: /ar/net/aspose.cells.lowcode/splitpartinfo/sheetname/
---
## SplitPartInfo.SheetName property

اسم الورقة التي يتواجد فيها الجزء الحالي.

```csharp
public string SheetName { get; }
```

### ملاحظات

قد تكون null في بعض الحالات، مثل عند تحويل المصنف بالكامل إلى صورة TIFF.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;
    using System.Reflection;

    public class SplitPartInfoPropertySheetNameDemo
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

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


