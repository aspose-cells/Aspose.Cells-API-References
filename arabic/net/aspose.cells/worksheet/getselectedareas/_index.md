---
title: "Worksheet.GetSelectedAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحصل على النطاقات المحددة من الخلايا في جدول البيانات المصمم"
type: docs
url: /ar/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

يحصل على النطاقات المختارة من الخلايا في جدول البيانات المصمم.

```csharp
public Range[] GetSelectedAreas()
```

### قيمة الإرجاع

يرجع جميع النطاقات المحددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تحديد نطاقات متعددة
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // الحصول على المناطق المحددة
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // عرض معلومات حول المناطق المحددة
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // مسح الاختيارات وتحديد نطاق واحد
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // الحصول على المنطقة المحددة الوحيدة
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


