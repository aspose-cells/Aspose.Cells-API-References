---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تنفذ هذه الواجهة للحصول على DrawObject و Bound أثناء التصيير"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

تنفذ هذه الواجهة للحصول على DrawObject و Bound أثناء التصيير.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
    {
        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
            }
        }

        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات النموذجية والأشكال
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // إنشاء مثيل PaginatedSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // اعرض القيمة الحالية للخاصية (يجب أن تكون null في البداية)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // عيّن معالج حدث مخصص جديد
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // سيؤدي هذا إلى استدعاء طريقة Draw أثناء التصيير
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // غيّر معالج الحدث إلى null لتوضيح الفرق
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


