---
title: "SheetRender.SheetRender"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ SheetRender. إنشاء SheetRender يحتاج إلى worksheet و ImageOrPrintOptions كمعلمات"
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

إنشاء SheetRender، يحتاج إلى ورقة عمل و ImageOrPrintOptions كمعلمات

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ورقة العمل | ورقة العمل | حدد أي جدول بيانات سيتم عرضه. |
| خيارات | ImageOrPrintOptions | ImageOrPrintOptions يحتوي على بعض خصائص صورة الإخراج |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // أنشئ دفتر عمل وأضف بعض البيانات النموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء خيارات الصورة/الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // أنشئ SheetRender باستخدام Worksheet و ImageOrPrintOptions
            SheetRender render = new SheetRender(worksheet, options);

            // إخراج عدد الصفحات
            Console.WriteLine("Page count: " + render.PageCount);

            // احفظ الصورة المعروضة
            render.ToImage(0, "output.png");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


