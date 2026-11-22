---
title: "PptxSaveOptions.AdjustFontSizeForRowType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PptxSaveOptions. تمثل نوع الخط الذي يحتاج إلى تعديل حجم الخط إذا كان ارتفاع الصف صغيرًا"
type: docs
url: /ar/net/aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/
---
## PptxSaveOptions.AdjustFontSizeForRowType property

تمثل نوع الخط الذي يحتاج إلى تعديل حجم الخط إذا كان ارتفاع الصف صغيرًا.

```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات والصفوف الفارغة
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue(""); // Empty row
            worksheet.Cells["A4"].PutValue("Data 2");
            
            // إنشاء خيارات حفظ PPTX
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows;
            
            // حفظ إلى PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("File saved with AdjustFontSizeForRowType setting");
        }
    }
}
```

### انظر أيضًا

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


