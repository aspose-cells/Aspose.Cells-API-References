---
title: "Class Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Column class. يمثل عمودًا واحدًا في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/column/
---
## Column class

يمثل عمودًا واحدًا في ورقة العمل.

```csharp
public class Column
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | يحصل على مستوى المجموعة للعمود. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | يشير إلى ما إذا كان هذا العمود يحتوي على إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من المصنف). |
| [Index](../../aspose.cells/column/index/) { get; } | يحصل على فهرس هذا العمود. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | ما إذا كان العمود مطويًا |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | يشير إلى ما إذا كان العمود مخفيًا. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) يحصل على نمط هذا العمود. |
| [Width](../../aspose.cells/column/width/) { get; set; } | يحصل على ويضبط عرض العمود بوحدة الأحرف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | يطبق التنسيقات على عمود كامل. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | يحصل على نمط هذا العمود. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | يضبط نمط هذا العمود. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة نمط جديد إلى المصنف
            Style style = workbook.CreateStyle();

            // تعيين لون الخلفية إلى الأزرق
            style.BackgroundColor = Color.Blue;

            // تعيين لون المقدمة إلى الأحمر
            style.ForegroundColor = Color.Red;

            // تعيين نمط الخلفية
            style.Pattern = BackgroundType.DiagonalStripe;

            // علامة النمط الجديد
            StyleFlag styleFlag = new StyleFlag();

            // ضبط جميع الأنماط
            styleFlag.All = true;

            // احصل على العمود الأول
            Column column = worksheet.Cells.Columns[0];

            // تطبيق النمط على العمود الأول
            column.ApplyStyle(style, styleFlag);

            // ضبط الخصائص الإضافية
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // حفظ ملف Excel
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


