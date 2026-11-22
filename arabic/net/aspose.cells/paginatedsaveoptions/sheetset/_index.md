---
title: "PaginatedSaveOptions.SheetSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تحصل أو تعيين الأوراق التي سيتم تصييرها. الافتراضي هو جميع الأوراق الظاهرة في دفتر العمل Visible"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/sheetset/
---
## PaginatedSaveOptions.SheetSet property

يحصل أو يحدد الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق الظاهرة في دفتر العمل: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد يحتوي على ورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // اضبط بعض البيانات النموذجية في كلا الورقتين
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // احفظ الورقة الثانية فقط باستخدام SheetSet
            pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
            
            // احفظ المصنف مع الأوراق المحددة
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


