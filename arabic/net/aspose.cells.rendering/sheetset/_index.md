---
title: "الفئة SheetSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.SheetSet. تصف مجموعة من الأوراق"
type: docs
url: /ar/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

يصف مجموعة من الأوراق.

```csharp
public class SheetSet
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | ينشئ مجموعة أوراق بناءً على فهارس الأوراق الدقيقة. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | ينشئ مجموعة أوراق بناءً على أسماء الأوراق الدقيقة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | يحصل على مجموعة تحتوي على الورقة النشطة في المصنف. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | يحصل على مجموعة تحتوي على جميع أوراق المصنف بترتيبها الأصلي. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | يحصل على مجموعة تحتوي على الأوراق المرئية في المصنف بترتيبها الأصلي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // إنشاء كائن PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // تعيين خاصية SheetSet لتشمل الورقة النشطة فقط
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // حفظ المصنف إلى ملف PDF
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // قم بتعيين خاصية SheetSet لتشمل جميع الأوراق الظاهرة
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // حفظ المصنف إلى ملف PDF
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // قم بتعيين خاصية SheetSet لتشمل جميع الأوراق
            pdfSaveOptions.SheetSet = SheetSet.All;

            // حفظ المصنف إلى ملف PDF
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


