---
title: "فئة SheetPrintingPreview"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Rendering.SheetPrintingPreview. معاينة طباعة ورقة العمل"
type: docs
url: /ar/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

معاينة طباعة ورقة العمل.

```csharp
public class SheetPrintingPreview
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | بنية SheetPrintingPreview |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | تقييم العدد الإجمالي للصفحات في ورقة العمل هذه |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // تحميل دفتر عمل موجود
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // احصل على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // إنشاء نسخة من SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // تقييم وطباعة العدد الإجمالي للصفحات في ورقة العمل
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


