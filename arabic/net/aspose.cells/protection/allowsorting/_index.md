---
title: "Protection.AllowSorting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان خيار الفرز مسموحًا به في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

يمثل ما إذا كان خيار الفرز مسموحًا به في ورقة عمل محمية.

```csharp
public bool AllowSorting { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تمكين حماية ورقة العمل
            worksheet.Protect(ProtectionType.All);
            
            // ضبط خصائص الحماية بما في ذلك AllowSorting
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // إخراج إعدادات الحماية
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // عرض قدرة الفرز
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


