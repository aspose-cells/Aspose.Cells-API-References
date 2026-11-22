---
title: "Cells.MinColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. الحد الأدنى لمؤشر العمود لتلك الخلايا التي تم إنشاءها في المجموعة لا يشمل العمود الذي تم تعريف النمط له لكامل العمود ولكن لم يتم إنشاء أي خلية فيه"
type: docs
url: /ar/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

الحد الأدنى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له للعمود بأكمله ولكن لم يتم إنشاء أي خلية فيه).

```csharp
public int MinColumn { get; }
```

### ملاحظات

تحتاج هذه الخاصية إلى التكرار والتحقق من الخلايا والصفوف بشكل ديناميكي، لذا فهي عملية تستغرق وقتًا ويجب عدم استدعائها بشكل متكرر، مثل استخدامها مباشرةً كشرط في حلقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مجموعة الخلايا
            Cells cells = worksheet.Cells;
            
            // املأ بعض البيانات في الأعمدة 2، 3 و4 (B, C, D)
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // احصل على الحد الأدنى لمؤشر العمود الذي يحتوي على بيانات
            int minColumn = cells.MinColumn;
            
            // احصل على الحد الأقصى لمؤشر العمود الذي يحتوي على بيانات
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // امسح العمود B لتوضيح تغيير MinColumn
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


