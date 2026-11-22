---
title: "Cells.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل وتضبط النمط الافتراضي لورقة العمل"
type: docs
url: /ar/net/aspose.cells/cells/style/
---
## Cells.Style property

يحصل ويعيّن النمط الافتراضي لورقة العمل.

```csharp
public Style Style { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // عيّن قيمة في الخلية A1
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // احصل على النمط الافتراضي وعدّل تنسيقه
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // تطبيق النمط المعدل على الخلية
            cell.SetStyle(style);

            // اعرض قيمة السلسلة المنسقة
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


