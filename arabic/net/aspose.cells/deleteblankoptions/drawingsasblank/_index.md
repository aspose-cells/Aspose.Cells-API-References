---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DeleteBlankOptions. تشير إلى ما إذا كانت الكائنات المرتبطة بالرسومات مثل الصورة الشكل المخطط... ستُعتبر كفارغة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... ستُعامل كفارغة. القيمة الافتراضية هي true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### ملاحظات

عند ضبط هذه الخاصية كـ false، لن تُعتبر جميع الصفوف/الأعمدة التي تغطيها كائنات الرسم كفارغة ولن يتم حذفها.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // أضف كائن رسم لاختبار سلوك DrawingsAsBlank
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // حذف الأعمدة الفارغة مع DrawingsAsBlank = false (يحافظ على الرسومات)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### انظر أيضًا

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


