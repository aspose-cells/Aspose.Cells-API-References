---
title: "ImageConverter.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ImageConverter. يحول ملف القالب إلى صور"
type: docs
url: /ar/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

يحول ملف القالب إلى صور.

```csharp
public static void Process(string templateFile, string resultFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | String | ملف القالب الذي سيتم تحويله إلى صور. |
| resultFile | String | ملف النتيجة (نمط الاسم) للصور المولدة. |

### ملاحظات

سيتم بناء ملفات الإخراج من ملف النتيجة المحدد عن طريق إلحاق رقم تسلسلي للورقة والجزء المقسم. على سبيل المثال، إذا كان ملف الإخراج المحدد هو Image.png، فستكون ملفات الصور المولدة Image_0_0.png، Image_0_1.png، …، Image_1_0.png، …

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد وتعبئته ببيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // حفظ كملف قالب للمعالجة
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // تحويل القالب إلى صور باستخدام معلمات (String, String)
                ImageConverter.Process("Template.xlsx", "OutputSheet.png");

                Console.WriteLine("Process method executed successfully. Generated image(s) from spreadsheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image conversion: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

يحول ملف القالب إلى صور

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | خيارات الإدخال والتحميل |
| saveOptions | LowCodeSaveOptions | خيارات الإخراج والحفظ |

### ملاحظات

عند التحويل إلى صورة بتنسيق يدعم صفحات متعددة (مثل tiff)، سيتم استخدام [`OutputFile`](../../lowcodesaveoptions/outputfile/) أو [`OutputStream`](../../lowcodesaveoptions/outputstream/) المحدد مباشرةً للصورة الناتجة. بالنسبة لأنواع الصور الأخرى، إذا كانت خيارات الحفظ قد حددت Stream كمخرج، فسيتم حفظ جميع الصور الناتجة إلى نفس الـ Stream. وإلا، سيتم بناء ملفات الإخراج من ملف الإخراج المحدد في خيارات الحفظ عن طريق إلحاق رقم تسلسلي للورقة والجزء المقسم. على سبيل المثال، إذا كان ملف الإخراج المحدد هو Image.png، فستكون ملفات الصور المولدة Image_0_0.png، Image_0_1.png، …، Image_1_0.png، …

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            try
            {
                // تهيئة LowCodeLoadOptions بملف قالب
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // تهيئة LowCodeSaveOptions بدليل الإخراج
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // تنفيذ طريقة Process بالمعلمات المحددة
                ImageConverter.Process(loadOptions, saveOptions);
                
                Console.WriteLine("Spreadsheet converted to images successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during processing: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

يحول ملف القالب إلى صور

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | خيارات الإدخال والتحميل |
| saveOptions | LowCodeSaveOptions | خيارات الحفظ. مخرجه ([`OutputFile`](../../lowcodesaveoptions/outputfile/) أو [`OutputStream`](../../lowcodesaveoptions/outputstream/)) لا تأثير له لأن جميع المخرجات سيتم تحديدها بواسطة معامل "provider" |
| provider | AbstractLowCodeSaveOptionsProvider | مزود خيارات الحفظ لحفظ الصور المولدة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
            const string templatePath = "SampleTemplate.xlsx";
            const string outputDir = "Output/";
            
            // إنشاء قالب عينة
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // تهيئة خيارات التحميل
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // تكوين خيارات الحفظ باستخدام LowCodeImageSaveOptions
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // استدعاء الطريقة الثابتة Process
                ImageConverter.Process(loadOptions, saveOptions, provider);
                Console.WriteLine($"Generated PNG images in: {Path.GetFullPath(outputDir)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Processing failed: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string path)
        {
            using (Workbook wb = new Workbook())
            {
                Worksheet sheet = wb.Worksheets[0];
                sheet.Cells["A1"].PutValue("LowCode Process Demo");
                sheet.Cells["B3"].PutValue(DateTime.Now.ToString());
                wb.Save(path, SaveFormat.Xlsx);
            }
        }

        private class DynamicSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            private readonly LowCodeImageSaveOptions _baseOptions; // Corrected type

            public DynamicSaveOptionsProvider(LowCodeImageSaveOptions options)
            {
                _baseOptions = options;
            }

            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // الوصول إلى خصائص الدقة من LowCodeImageSaveOptions
                if (partInfo.SheetIndex == 0)
                {
                    _baseOptions.ImageOptions.HorizontalResolution = 300;
                    _baseOptions.ImageOptions.VerticalResolution = 300;
                }
                return _baseOptions;
            }
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


