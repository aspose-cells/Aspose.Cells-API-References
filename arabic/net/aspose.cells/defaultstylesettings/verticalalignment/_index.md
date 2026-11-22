---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DefaultStyleSettings. تحصل/تضبط القيمة الافتراضية للمحاذاة العمودية"
type: docs
url: /ar/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

الحصول/تعيين القيمة الافتراضية للمحاذاة العمودية

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين المحاذاة العمودية الافتراضية إلى الأسفل
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين بعض البيانات النموذجية
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // تحقق من تطبيق المحاذاة العمودية على جميع الخلايا
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // احفظ المصنف
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


