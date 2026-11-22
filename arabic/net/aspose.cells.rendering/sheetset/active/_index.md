---
title: "SheetSet.Active"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SheetSet. تحصل على مجموعة تحتوي على الورقة النشطة في دفتر العمل"
type: docs
url: /ar/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

يحصل على مجموعة تحتوي على الورقة النشطة في المصنف.

```csharp
public static SheetSet Active { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد يحتوي على ورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // تعيين ورقة العمل الثانية كنشطة
            workbook.Worksheets.ActiveSheetIndex = 1;

            // إضافة بيانات إلى ورقتي العمل
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // أنشئ خيارات حفظ PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // حفظ الورقة النشطة فقط
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // حفظ جميع الأوراق للمقارنة
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


