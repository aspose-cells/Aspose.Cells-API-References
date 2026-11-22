---
title: "Cell.SharedStyleIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل على فهرس النمط المشترك للخلية في مجموعة الأنماط"
type: docs
url: /ar/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

يحصل على فهرس النمط المشترك للخلية في مجموعة الأنماط.

```csharp
public int SharedStyleIndex { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط وتعيين بعض الخصائص
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // تطبيق النمط على الخلية A1
            worksheet.Cells["A1"].SetStyle(style);

            // احصل على فهرس النمط المشترك للخلية A1
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // استرجاع النمط من مجموعة الأنماط باستخدام الفهرس
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // إخراج معلومات النمط للتحقق
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


