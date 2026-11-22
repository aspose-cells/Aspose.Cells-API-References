---
title: "WorkbookDesigner.UpdateReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. تشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

يشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها.

```csharp
public bool UpdateReference { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // إنشاء مجموعة بيانات نموذجية
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ID", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Price", typeof(decimal));
            
            dt.Rows.Add(1, "Product A", 19.99);
            dt.Rows.Add(2, "Product B", 29.99);
            dt.Rows.Add(3, "Product C", 39.99);
            
            ds.Tables.Add(dt);

            // إنشاء مصمم مصنف
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // تعيين خاصية UpdateReference إلى true
            designer.UpdateReference = true;
            
            // إنشاء مصنف جديد باستخدام قالب
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة علامات ذكية
            worksheet.Cells["A1"].PutValue("&=Products.ID");
            worksheet.Cells["B1"].PutValue("&=Products.Name");
            worksheet.Cells["C1"].PutValue("&=Products.Price");
            
            designer.Workbook = workbook;
            designer.SetDataSource("Products", dt);
            
            // معالجة المصمم
            designer.Process();
            
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


