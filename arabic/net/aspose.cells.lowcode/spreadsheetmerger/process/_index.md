---
title: "SpreadsheetMerger.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SpreadsheetMerger. دمج ملفات القالب المعطاة"
type: docs
url: /ar/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

دمج ملفات القالب المحددة.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFiles | String[] | ملفات القالب التي سيتم دمجها |
| resultFile | String | الملف الناتج |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithStringArrayStringDemo
    {
        public static void Run()
        {
            // إنشاء ملفات قالب نموذجية
            CreateTemplateFile("template1.xlsx", "Data from Template 1");
            CreateTemplateFile("template2.xlsx", "Data from Template 2");

            string[] templateFiles = { "template1.xlsx", "template2.xlsx" };
            string resultFile = "merged_output.xlsx";

            try
            {
                SpreadsheetMerger.Process(templateFiles, resultFile);

                Console.WriteLine($"Process method merged {templateFiles.Length} files into {resultFile}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### انظر أيضًا

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

يدمج ملفات القالب المتعددة في ملف واحد.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | LowCodeMergeOptions | خيارات دمج الملفات |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithLowCodeMergeOptDemo
    {
        public static void Run()
        {
            // تحضير ملفي قالب بسيطين سيتم دمجهما.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // إنشاء مثيل من فئة الخيارات.
                // الفئة LowCodeMergeOptions هي جزء من Aspose.Cells.LowCode.
                // في هذا العرض التجريبي نستخدم المُنشئ الافتراضي.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // استدعِ طريقة Process التي تقبل LowCodeMergeOptions.
                SpreadsheetMerger.Process(options);

                Console.WriteLine("Process method invoked successfully with LowCodeMergeOptions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### انظر أيضًا

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


