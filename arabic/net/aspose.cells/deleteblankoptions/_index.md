---
title: "فئة DeleteBlankOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.DeleteBlankOptions. تمثل إعداد حذف الخلايا/الصفوف/الأعمدة الفارغة."
type: docs
url: /ar/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

يمثل إعداد حذف الخلايا/الصفوف/الأعمدة الفارغة.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... ستُعامل كفارغة. القيمة الافتراضية هي true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون صيغة والنتيجة المحسوبة هي null أو سلسلة فارغة. القيمة الافتراضية هي false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | يشير إلى ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون قيمتها سلسلة فارغة. القيمة الافتراضية هي true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي سيتم فحصه وحذف الصفوف/الأعمدة الفارغة. القيمة الافتراضية هي -1 و -1 تعني النطاق الأقصى لجميع الكائنات (الخلايا، الرسومات، ...) التي تحتاج إلى الفحص. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | يحصل/يضبط المراقب لتتبع التغييرات التي تسببها عملية الحذف.(موروث من [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | يحدد فهرس الصف/العمود الابتدائي للنطاق الذي سيتم فحصه وحذف الصف/العمود الفارغ. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق عمل أخرى.(موروث من [`DeleteOptions`](../deleteoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ ورقة العمل ببعض البيانات
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // إنشاء مثال من DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // حذف الصفوف الفارغة بناءً على الخيارات
            worksheet.Cells.DeleteBlankRows(options);

            // احفظ المصنف
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


