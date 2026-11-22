---
title: "PdfConverter.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PdfConverter. يحول ملف القالب المعطى إلى pdf"
type: docs
url: /ar/net/aspose.cells.lowcode/pdfconverter/process/
---
## Process(string, string) {#process_1}

يقوم بتحويل ملف القالب المحدد إلى pdf.

```csharp
public static void Process(string templateFile, string resultFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | String | ملف القالب الذي سيتم تحويله |
| resultFile | String | الملف الناتج، يجب أن يكون ملف pdf. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class PdfConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء ملف قالب تجريبي
            CreateSampleTemplate("template.xlsx");

            try
            {
                // استدعاء طريقة Process مع معاملات (String, String) مباشرةً على النوع
                PdfConverter.Process("template.xlsx", "output.pdf");
                
                Console.WriteLine("Successfully converted template.xlsx to output.pdf");
                Console.WriteLine($"PDF created at: {Path.GetFullPath("output.pdf")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateSampleTemplate(string fileName)
        {
            using (Workbook workbook = new Workbook())
            {
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("PDF Conversion Test");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
                workbook.Save(fileName);
            }
        }
    }
}
```

### انظر أيضًا

* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

يقوم بتحويل ملف القالب إلى pdf

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | خيارات الإدخال والتحميل |
| saveOptions | LowCodeSaveOptions | خيارات الإخراج والحفظ |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class PdfConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // إنشاء دفق إدخال تجريبي (ملف Excel في الذاكرة)
            var workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Content");
            MemoryStream template = new MemoryStream();
            workbook.Save(template, SaveFormat.Xlsx);
            template.Position = 0;

            // دليل الإخراج
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // مثال 1: التحويل إلى PDF
            Aspose.Cells.LowCode.PdfConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodePdfSaveOptions() 
                { 
                    OutputFile = outputDir + "output.pdf",
                    PdfOptions = new PdfSaveOptions()
                });

            // مثال 2: تحويل إلى HTML
            Aspose.Cells.LowCode.HtmlConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodeSaveOptions() 
                { 
                    OutputFile = outputDir + "output.html" 
                });

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


