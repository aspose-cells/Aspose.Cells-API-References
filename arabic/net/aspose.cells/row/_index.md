---
title: "الفئة Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Row. تمثل صفًا واحدًا في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/row/
---
## Row class

يمثل صفًا واحدًا في ورقة العمل.

```csharp
public class Row : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | يحصل على أول كائن خلية في الصف. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | يحصل على أول خلية غير فارغة في الصف. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | يحصل على مستوى المجموعة للصف. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | يشير إلى ما إذا كان هذا الصف يحتوي على إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من المصنف). |
| [Height](../../aspose.cells/row/height/) { get; set; } | يسترجع ويعيّن ارتفاع الصف بوحدة النقاط. |
| [Index](../../aspose.cells/row/index/) { get; } | يسترجع فهرس هذا الصف. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | يشير إلى ما إذا كان الصف يحتوي على أي بيانات |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | ما إذا كان الصف مطويًا |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. قيمة true لهذه الخاصية تعني أيضًا أن ارتفاع الصف "تلقائي" دون قيمة ارتفاع مخصصة تم تعيينها من قبل المستخدم. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | يشير إلى ما إذا كان الصف مخفيًا. |
| [Item](../../aspose.cells/row/item/) { get; } | يسترجع الخلية. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | يسترجع آخر كائن خلية في الصف. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | يسترجع آخر خلية غير فارغة في الصف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | يطبق التنسيقات على الصف بأكمله. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | نسخ إعدادات الصف، مثل النمط، الارتفاع، الظهور، ...إلخ. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع آخر. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع كائن صف آخر. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | احصل على الخلية بواسطة فهرس محدد في مجموعة الخلايا لهذا الصف. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | يسترجع الخلية أو null في الفهرس المحدد. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | يسترجع عداد الخلايا |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | يسترجع عدادًا يتنقل عبر الخلايا في هذا الصف. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | يسترجع نمط هذا الصف. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | يضبط نمط هذا الصف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن نمط
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

            // احصل على الصف الأول
            Row row = worksheet.Cells.Rows[0];

            // تطبيق النمط على الصف الأول
            row.ApplyStyle(style, styleFlag);

            // ضبط خصائص الصف
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // الوصول إلى الخلايا في الصف
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // التحقق مما إذا كان الصف فارغًا
            bool isBlank = row.IsBlank;

            // التحقق مما إذا كان الصف يحتوي على نمط مخصص
            bool hasCustomStyle = row.HasCustomStyle;

            // الحصول على فهرس الصف
            int rowIndex = row.Index;

            // الحصول على خلية حسب الفهرس
            Cell cellByIndex = row.GetCellByIndex(0);

            // الحصول على نمط الصف
            Style rowStyle = row.GetStyle();

            // ضبط نمط الصف
            row.SetStyle(rowStyle);

            // نسخ الإعدادات من صف آخر
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // التعداد عبر الخلايا في الصف
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // حفظ ملف Excel
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


