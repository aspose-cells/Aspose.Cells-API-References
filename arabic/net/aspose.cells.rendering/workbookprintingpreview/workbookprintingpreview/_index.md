---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ WorkbookPrintingPreview. إنشاء WorkbookPrintingPreview"
type: docs
url: /ar/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

بنية WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصنف | المصنف | حدد أي دفتر عمل سيتم طباعته. |
| خيارات | ImageOrPrintOptions | ImageOrPrintOptions يحتوي على بعض خصائص الإخراج |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // حدد خيارات الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // أنشئ معاينة الطباعة باستخدام دفتر العمل والخيارات
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // اعرض عدد الصفحات
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


