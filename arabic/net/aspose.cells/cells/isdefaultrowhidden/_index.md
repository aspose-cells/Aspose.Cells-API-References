---
title: "Cells.IsDefaultRowHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تشير إلى ما إذا كان الصف مخفيًا افتراضيًا"
type: docs
url: /ar/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

يشير إلى ما إذا كان الصف مخفيًا بشكل افتراضي.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين خاصية إخفاء الصف الافتراضي
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // عرض القيمة الحالية لـ IsDefaultRowHidden
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


