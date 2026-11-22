---
title: "PclSaveOptions.EmbedFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PclSaveOptions. تشير إلى ما إذا كان يجب تضمين الخط في ملف Pcl الناتج."
type: docs
url: /ar/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

يشير إلى ما إذا كان يجب تضمين الخط في ملف Pcl الناتج.

```csharp
public bool EmbedFont { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وإضافة بعض البيانات النموذجية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // إنشاء خيارات حفظ PCL
                PclSaveOptions pclOptions = new PclSaveOptions();

                // اقرأ واعرض القيمة الحالية لخاصية EmbedFont.
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (اختياري) إذا كانت الخاصية قابلة للكتابة يمكنك تعيينها، لكننا نقرأها فقط هنا.
                // pclOptions.EmbedFont = true;

                // احفظ المصنف كملف PCL باستخدام الخيارات
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


