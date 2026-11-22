---
title: "SheetSet.Visible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SheetSet. تُرجع مجموعة تحتوي على الأوراق الظاهرة لدفتر العمل بترتيبها الأصلي"
type: docs
url: /ar/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

يحصل على مجموعة تحتوي على الأوراق المرئية في المصنف بترتيبها الأصلي.

```csharp
public static SheetSet Visible { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد يحتوي على ورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // إخفاء ورقة العمل الثانية
            workbook.Worksheets[1].IsVisible = false;

            // إعداد خيارات الحفظ لتصدير الأوراق الظاهرة فقط
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // حفظ دفتر العمل (سيتم تصدير الورقة الظاهرة فقط)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### انظر أيضًا

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


