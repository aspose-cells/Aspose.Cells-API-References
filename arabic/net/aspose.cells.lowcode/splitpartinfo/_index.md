---
title: "الفئة SplitPartInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LowCode.SplitPartInfo. تمثل معلومات إدخال/إخراج واحد لعدة إدخالات/إخراجات مثل الصفحة الحالية التي سيتم عرضها عند تحويل جدول البيانات إلى صورة"
type: docs
url: /ar/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

يمثل معلومات إدخال/إخراج واحد للعديد من الإدخالات/الإخراجات، مثل الصفحة الحالية التي سيتم عرضها عند تحويل جدول البيانات إلى صورة.

```csharp
public class SplitPartInfo
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | فهرس الجزء الحالي في التسلسل (مبني على الصفر). -1 يعني عدم وجود أجزاء متعددة وبالتالي النتيجة واحدة. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | فهرس الورقة التي يتواجد فيها الجزء الحالي. -1 يدل على وجود ورقة واحدة فقط. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | اسم الورقة التي يتواجد فيها الجزء الحالي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مصنف يحتوي على عدة أوراق للعرض
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // إنشاء LowCodeLoadOptions و LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // إنشاء موفر مخصص لعرض استخدام SplitPartInfo
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // معالجة عملية التقسيم
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // عرض الوصول إلى خصائص SplitPartInfo
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


