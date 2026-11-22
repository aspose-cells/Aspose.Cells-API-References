---
title: "Protection.AllowDeletingColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان مسموحًا بحذف الأعمدة في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

يمثل ما إذا كان حذف الأعمدة مسموحًا به في ورقة عمل محمية.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### ملاحظات

يجب أن تكون الأعمدة التي تحتوي على الخلايا المراد حذفها غير مقفلة عندما تكون الورقة محمية، ويجب تمكين خيار "Select unlocked cells".

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تمكين حماية ورقة العمل
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // تحقق من الإعداد
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // حاول حذف عمود (يجب أن يعمل لأن AllowDeletingColumn صحيح)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // تعطيل حذف الأعمدة
            protection.AllowDeletingColumn = false;

            // حاول حذف عمود آخر (يجب أن يفشل)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


