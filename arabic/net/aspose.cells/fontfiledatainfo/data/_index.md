---
title: "FontFileDataInfo.Data"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontFileDataInfo. يحصل على البيانات الثنائية لملف الخط"
type: docs
url: /ar/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

يحصل على البيانات الثنائية لملف الخط.

```csharp
public byte[] Data { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // حمّل ملف خط (استبدله بمسار ملف الخط الفعلي)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // أنشئ كائن FontConfigs وأضف الخط
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // في الاستخدام الفعلي، سيتم الحصول على FontFileDataInfo من المكتبة
            // لأغراض العرض، سنظهر فقط كيف يمكنك استخدامه إذا كان لديك واحد
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // اعرض معلومات حول بيانات الخط (إن وجدت)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // في الاستخدام الفعلي، سيتم استخدام خاصية Data للوصول إلى البيانات الثنائية للخط
            // على سبيل المثال، قد تقوم بحفظه إلى ملف:
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // احفظ دفتر العمل (سيؤثر الخط على العرض إذا استُخدم في الخلايا)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


