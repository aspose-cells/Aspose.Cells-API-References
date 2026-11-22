---
title: "Cells.StandardWidthPixels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. الحصول على أو تعيين عرض العمود الافتراضي في ورقة العمل بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل.

```csharp
public int StandardWidthPixels { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين والحصول على العرض القياسي بالبكسل
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // تعيين والحصول على العرض القياسي بالأحرف
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // تعيين والحصول على الارتفاع القياسي بالنقاط
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


