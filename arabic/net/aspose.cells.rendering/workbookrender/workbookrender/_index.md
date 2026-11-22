---
title: "WorkbookRender.WorkbookRender"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ WorkbookRender. بنية WorkbookRender"
type: docs
url: /ar/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

بناء WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصنف | المصنف | تحديد أي دفتر عمل سيتم عرضه. |
| خيارات | ImageOrPrintOptions | ImageOrPrintOptions يحتوي على بعض خصائص صورة الإخراج |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // إنشاء خيارات الصورة/الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // إنشاء مُصوّر دفتر العمل
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // إخراج عدد الصفحات
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


