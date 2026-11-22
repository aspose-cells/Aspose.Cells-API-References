---
title: "HtmlSaveOptions.ExportArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تحصل أو تعيين منطقة الخلية (CellArea) التي سيتم تصديرها للورقة النشطة الحالية. إذا قمت بتعيين هذه الخاصية، سيتم حذف منطقة الطباعة للورقة النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف كـ HTML."
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

يحصل على أو يضبط CellArea المُصدَّر لورقة العمل النشطة الحالية. إذا قمت بتعيين هذه السمة، سيتم حذف منطقة الطباعة لورقة العمل النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى html.

```csharp
public CellArea ExportArea { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات في ورقة العمل
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // تعيين خيارات حفظ HTML مع منطقة التصدير
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // احفظ دفتر العمل مع منطقة التصدير المحددة
            workbook.Save("output.html", options);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


