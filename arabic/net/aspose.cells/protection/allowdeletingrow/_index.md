---
title: "Protection.AllowDeletingRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان حذف الصفوف مسموحًا به في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

يمثل ما إذا كان حذف الصفوف مسموحًا به في ورقة عمل محمية.

```csharp
public bool AllowDeletingRow { get; set; }
```

### ملاحظات

يجب إلغاء قفل الصفوف التي تحتوي على الخلايا التي سيتم حذفها عندما تكون الورقة محمية، ويجب تمكين خيار "Select unlocked cells".

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ضبط إعدادات الحماية
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // حماية ورقة العمل
            sheet.Protect(ProtectionType.All);

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تحميل المصنف المحفوظ للتحقق من الإعدادات
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // تحقق من AllowDeletingRow والخصائص الأخرى
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


