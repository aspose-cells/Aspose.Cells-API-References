---
title: "SplitPartInfo.PartIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SplitPartInfo. فهرس الجزء الحالي في تسلسل يبدأ من الصفر. 1 يعني أنه لا توجد أجزاء متعددة وبالتالي النتيجة واحدة"
type: docs
url: /ar/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

فهرس الجزء الحالي في التسلسل (مبني على الصفر). -1 يعني عدم وجود أجزاء متعددة وبالتالي النتيجة واحدة.

```csharp
public int PartIndex { get; }
```

### ملاحظات

إذا كان من الضروري معالجة عدة أوراق وكل ورقة تُعالج (تقسيم) بشكل منفصل، فإن فهرس الجزء يبدأ دائمًا من 0 لكل ورقة. على سبيل المثال، عند تحويل المصنف إلى صور، يمثل فهرس صفحة الإخراج للورقة التي تتم معالجتها حاليًا. و -1 يدل على وجود صفحة واحدة فقط للورقة الحالية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مصنف يحتوي على عدة أوراق
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // حفظ المصنف لاستخدامه في عملية التقسيم
                workbook.Save("sample.xlsx");

                // إنشاء خيارات التحميل
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // إنشاء خيارات التقسيم بمزود مخصص
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // معالجة عملية التقسيم
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // عرض قراءة خاصية PartIndex
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### انظر أيضًا

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


