---
title: "الفئة WorkbookPrintingPreview"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.WorkbookPrintingPreview. معاينة طباعة المصنف"
type: docs
url: /ar/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

معاينة طباعة المصنف.

```csharp
public class WorkbookPrintingPreview
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | بنية WorkbookPrintingPreview |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | تقييم العدد الإجمالي للصفحات في هذا المصنف |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // تحميل دفتر عمل موجود
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // إنشاء نسخة من ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // إنشاء كائن من WorkbookPrintingPreview
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // تقييم العدد الإجمالي للصفحات في المصنف
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // طباعة عدد الصفحات المُقَيَّم
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


