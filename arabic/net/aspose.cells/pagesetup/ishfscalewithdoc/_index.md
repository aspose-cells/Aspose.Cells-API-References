---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تشير إلى ما إذا كان الرأس والتذييل يتم تحجيمهما مع تحجيم المستند. ينطبق فقط على Excel 2007"
type: docs
url: /ar/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

يشير إلى ما إذا كانت الترويسة والتذييل يتم تحجيمهما مع تحجيم المستند. ينطبق فقط على Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين إعداد الصفحة الأساسي
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // عرض خاصية IsHFScaleWithDoc
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // احفظ المصنف
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


