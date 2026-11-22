---
title: "WorkbookDesigner.UpdateEmptyStringAsNull"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. إذا كان TRUE سيتم إدراج Null إذا كانت القيمة ..."
type: docs
url: /ar/net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

إذا كان TRUE، سيتم إدراج Null إذا كانت القيمة ""؛

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateEmptyStringAsNullDemo
    {
        public static void Run()
        {
            // إنشاء مجموعة بيانات عينة تحتوي على سلاسل فارغة
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("Name");
            dt.Columns.Add("Price");
            dt.Rows.Add("Laptop", "");
            dt.Rows.Add("", "999.99");
            ds.Tables.Add(dt);

            // إنشاء مصنف مع علامات المصمم
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Products.Name");
            worksheet.Cells["B1"].PutValue("&=$Products.Price");

            // تهيئة WorkbookDesigner وتعيين الخصائص
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
            
            // تعيين مصدر البيانات ومعالجته
            designer.SetDataSource(ds.Tables["Products"]);
            designer.Process();

            // تحقق من النتائج
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


