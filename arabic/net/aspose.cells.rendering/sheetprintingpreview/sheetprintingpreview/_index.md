---
title: "SheetPrintingPreview.SheetPrintingPreview"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ SheetPrintingPreview. بنية SheetPrintingPreview"
type: docs
url: /ar/net/aspose.cells.rendering/sheetprintingpreview/sheetprintingpreview/
---
## SheetPrintingPreview constructor

بنية SheetPrintingPreview

```csharp
public SheetPrintingPreview(Worksheet sheet, ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ورقة | ورقة العمل | حدد أي جدول بيانات سيتم طباعته. |
| خيارات | ImageOrPrintOptions | ImageOrPrintOptions يحتوي على بعض خصائص الإخراج |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewMethodctorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // إنشاء خيارات الصورة/الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // إنشاء معاينة طباعة الورقة
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            // إخراج عدد الصفحات المُقَيم
            Console.WriteLine($"Evaluated page count: {preview.EvaluatedPageCount}");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


