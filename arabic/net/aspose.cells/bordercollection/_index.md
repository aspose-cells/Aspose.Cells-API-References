---
title: "الفئة BorderCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.BorderCollection. يحتوي على مجموعة من كائنات Border"
type: docs
url: /ar/net/aspose.cells/bordercollection/
---
## BorderCollection class

يحتوي على مجموعة من كائنات [`Border`](../border/).

```csharp
public class BorderCollection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | يحصل أو يضبط Color للخطوط القطرية. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | يحصل أو يضبط نمط الخطوط القطرية. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق الحدود اليسرى، اليمنى، العليا والسفلى فقط على حدود الخلية الخارجية لنطاق الخلايا. القيمة الافتراضية هي true. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | يحصل على عنصر [`Border`](../border/) في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | يضبط Color لجميع الحدود في المجموعة. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | يضبط نمط جميع حدود المجموعة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderCollectionDemo
    {
        public static void BorderCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى كائن Workbook
            workbook.Worksheets.Add();

            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية "A1" من ورقة العمل
            Cell cell = worksheet.Cells["A1"];

            // إضافة قيمة إلى الخلية "A1"
            cell.PutValue("Visit Aspose!");

            // الحصول على نمط الخلية
            Style style = cell.GetStyle();

            // ضبط نمط الخط للحد العلوي
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // ضبط color للحد العلوي
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // ضبط نمط الخط للحد السفلي
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // ضبط color للحد السفلي
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // ضبط نمط الخط للحد الأيسر
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // ضبط color للحد الأيسر
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // ضبط نمط الخط للحد الأيمن
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // ضبط color للحد الأيمن
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // ضبط خصائص القطرية
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // حفظ ملف Excel
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


