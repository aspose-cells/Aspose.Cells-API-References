---
title: "DeleteBlankOptions.EndIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DeleteBlankOptions. تحدد فهرس الصف/العمود النهائي شامل النطاق للتحقق وحذف الصفوف/الأعمدة الفارغة. القيمة الافتراضية هي 1 و1 تعني النطاق الأقصى لجميع الكائنات/الخلايا/الرسومات ... التي تحتاج إلى الفحص"
type: docs
url: /ar/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي سيتم فحصه وحذف الصفوف/الأعمدة الفارغة. القيمة الافتراضية هي -1 و -1 تعني النطاق الأقصى لجميع الكائنات (الخلايا، الرسومات، ...) التي تحتاج إلى الفحص.

```csharp
public int EndIndex { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // املأ بعض الخلايا بالقيم
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // أنشئ خيارات الحذف بنطاق محدد
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // احذف الأعمدة الفارغة ضمن النطاق المحدد
            cells.DeleteBlankColumns(dbo);

            // أخرج النتائج لتوضيح تأثير EndIndex
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### انظر أيضًا

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


