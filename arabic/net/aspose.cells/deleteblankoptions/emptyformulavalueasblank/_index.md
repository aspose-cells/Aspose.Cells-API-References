---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DeleteBlankOptions. ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون صيغة والنتيجة المحسوبة null أو سلسلة فارغة. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون صيغة والنتيجة المحسوبة هي null أو سلسلة فارغة. القيمة الافتراضية هي false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### ملاحظات

بشكل عام يجب على المستخدم التأكد من أن الصيغ قد تم حسابها قبل عملية الحذف مع ضبط هذه الخاصية إلى true. وإلا سيتم اعتبار جميع الصيغ التي تم إنشاؤها حديثًا عبر واجهات برمجة التطبيقات العادية مثل [`Formula`](../../cell/formula/) كفراغ وقد تُحذف لأن نتائجها المحسوبة قبل الحساب كلها null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء بيانات عينة
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // حذف الصفوف الفارغة دون اعتبار فراغات الصيغ
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // إعادة تعيين البيانات
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // حذف الصفوف الفارغة مع اعتبار فراغات الصيغ كفارغة
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### انظر أيضًا

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


