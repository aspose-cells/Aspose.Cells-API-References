---
title: "FontFileDataInfo.FormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontFileDataInfo. يحصل على نوع تنسيق الخط لملف الخط"
type: docs
url: /ar/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

يحصل على نوع تنسيق الخط لملف الخط.

```csharp
public FontFileFormatType FormatType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض النص لتوضيح استخدام الخط
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // حمّل ملف خط تجريبي (استبدله بمسار ملف الخط الفعلي)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // سجّل مجلد الخط
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // في سيناريو واقعي، سيتم الحصول على FontFileDataInfo من المكتبة
                    // للعرض، سنحاكي الحصول على معلومات الخط
                    // ملاحظة: قد توفر الواجهة البرمجية الفعلية هذا عبر FontConfigs أو ما شابه
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // اعرض قيمة خاصية FormatType
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // اعرض قيمة التعداد كسلسلة
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // طبق الخط على خلية (مفهومي - قد تختلف التنفيذ الفعلي)
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // احفظ المصنف
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // طريقة مساعدة لمحاكاة الحصول على FontFileDataInfo
        // في الاستخدام الفعلي، سيُقدم هذا من قبل واجهة Aspose.Cells API
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // أنشئ كائنًا تجريبيًا من FontFileDataInfo (في الواقع، سيأتي هذا من الواجهة البرمجية)
                // نظرًا لعدم إمكانية إنشاءه مباشرةً، سنحاكي السلوك
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // في تنفيذ واقعي، سيُرجع هذا من الواجهة البرمجية
                // في هذا العرض التجريبي، سنعيد فقط null لأننا لا نستطيع إنشاء الكائن
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### انظر أيضًا

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


