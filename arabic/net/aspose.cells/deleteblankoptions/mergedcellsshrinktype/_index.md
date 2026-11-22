---
title: "DeleteBlankOptions.MergedCellsShrinkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DeleteBlankOptions. تشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة"
type: docs
url: /ar/net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### ملاحظات

بالنسبة إلى KeepHeaderOnly، سيتم اعتبار جميع الخلايا فيه كفارغة باستثناء الخلية العلوية اليسرى غير الفارغة. هذه هي القيمة الافتراضية لهذه الخاصية. بالنسبة إلى None، سيتم اعتبار جميع الخلايا فيه غير فارغة. بالنسبة إلى ShrinkToFit، سيتم اعتبار جميع الخلايا خارج منطقة عرض المحتوى كفارغة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // إعداد بيانات عينة مع خلايا مدمجة
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");
            
            // أنشئ خيارات الحذف بأنواع تقليص مختلفة
            DeleteBlankOptions options = new DeleteBlankOptions();
            
            // الحالة 1: KeepHeaderOnly
            options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // إعادة تعيين ورقة العمل
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // الحالة 2: ShrinkToFit
            options.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After ShrinkToFit - Merged area adjusted: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // إعادة تعيين ورقة العمل
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // الحالة 3: None
            options.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After None - Merged area unchanged: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
        }
    }
}
```

### انظر أيضًا

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


