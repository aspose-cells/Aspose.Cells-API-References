---
title: "WorkbookDesigner.RepeatFormulasWithSubtotal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. تشير إلى ما إذا كان يتم تكرار الصيغ مع صف المجموع الفرعي"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

يشير إلى ما إذا كانت الصيغ المتكررة مع صف المجموع الفرعي.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyRepeatFormulasWithSubtotalDemo
    {
        public static void Run()
        {
            // أنشئ DataTable نموذجية
            DataTable dt = new DataTable("products1");
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Quantity", typeof(int));
            
            // أضف بيانات تجريبية
            dt.Rows.Add(1, "Product A", 10.5m, 5);
            dt.Rows.Add(2, "Product B", 15.2m, 3);
            dt.Rows.Add(3, "Product C", 8.7m, 7);

            // إنشاء مصنف جديد بصيغة قالب
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إعداد القالب باستخدام العلامات الذكية والصيغة
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$UnitPrice");
            worksheet.Cells["D1"].PutValue("&=$Quantity");
            worksheet.Cells["E1"].PutValue("=SUM(C2:D2)"); // Formula to be repeated

            // إنشاء المصمم وتعيين RepeatFormulasWithSubtotal
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.RepeatFormulasWithSubtotal = true;
            designer.SetDataSource(dt);
            
            // معالجة القالب
            designer.Process();

            // تحقق من تكرار الصيغة لكل صف
            Console.WriteLine("Formula in E2: " + worksheet.Cells["E2"].Formula);
            Console.WriteLine("Formula in E3: " + worksheet.Cells["E3"].Formula);
            Console.WriteLine("Formula in E4: " + worksheet.Cells["E4"].Formula);

            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


