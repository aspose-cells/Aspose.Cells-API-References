---
title: "Workbook.GetFonts"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحصل على جميع الخطوط في مجموعة الأنماط"
type: docs
url: /ar/net/aspose.cells/workbook/getfonts/
---
## Workbook.GetFonts method

يحصل على جميع الخطوط في مجموعة الأنماط.

```csharp
public Font[] GetFonts()
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetFontsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء خلايا بخطوط مختلفة
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["A2"].PutValue("Sample Text 2");
            
            // احصل على الخطوط وعدلها
            Font font1 = worksheet.Cells["A1"].GetStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            
            Font font2 = worksheet.Cells["A2"].GetStyle().Font;
            font2.Name = "Times New Roman";
            font2.Size = 14;
            font2.IsBold = true;

            // احصل على جميع الخطوط المستخدمة في Workbook
            Font[] fonts = workbook.GetFonts();
            Console.WriteLine("Total fonts in workbook: " + fonts.Length);
            
            // عرض معلومات الخط
            foreach (Font font in fonts)
            {
                Console.WriteLine($"Font: {font.Name}, Size: {font.Size}, Bold: {font.IsBold}");
            }
            
            // احفظ وأعد التحميل لإظهار الاستمرارية
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Workbook loadedWorkbook = new Workbook(stream);
                Console.WriteLine("Fonts after save/load: " + loadedWorkbook.GetFonts().Length);
            }
        }
    }
}
```

### انظر أيضًا

* class [Font](../../font/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


