---
title: "SpreadsheetSplitter.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SpreadsheetSplitter. تقسم ملف القالب المعطى إلى أجزاء متعددة"
type: docs
url: /ar/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

يقسم ملف القالب المحدد إلى عدة أجزاء.

```csharp
public static void Process(string templateFile, string resultFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | String | ملف القالب المراد تقسيمه |
| resultFile | String | ملف الناتج (نمط الاسم) |

### ملاحظات

سيتم بناء ملفات الإخراج من الملف الناتج المحدد عن طريق إلحاق رقم تسلسل الورقة والجزء المقسوم. على سبيل المثال، إذا كان ملف الإخراج المحدد هو Split.xlsx، فستكون الملفات المولدة Split_0_0.xlsx، Split_0_1.xlsx، …، Split_1_0.xlsx، …

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع عدة أوراق عمل
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // حفظ كملف قالب
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // تحديد نمط إخراج النتيجة
            string resultPattern = "SplitResult_";
            
            try
            {
                // معالجة القالب مباشرةً باستخدام الطريقة الثابتة
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

يقسم ملف جدول البيانات إلى أجزاء متعددة.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | LowCodeSplitOptions | خيارات تقسيم جدول البيانات |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // تهيئة خيارات الانقسام
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // تنفيذ تقسيم جدول البيانات باستخدام طريقة ثابتة
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
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

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


