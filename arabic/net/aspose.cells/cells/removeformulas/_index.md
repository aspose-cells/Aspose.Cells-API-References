---
title: "Cells.RemoveFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تزيل جميع الصيغ وتستبدلها بقيمة الصيغة"
type: docs
url: /ar/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

يزيل جميع الصيغ ويستبدلها بقيمة الصيغة.

```csharp
public void RemoveFormulas()
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveFormulasDemo
    {
        public static void Run()
        {
            // إنشاء مجموعة بيانات نموذجية
            DataSet ds = new DataSet();

            // إنشاء وتعبئة جدول Master
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // إنشاء وتعبئة جدول OppLineItems
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // إنشاء دفتر عمل جديد
            Workbook wkb = new Workbook();
            
            // استخدام WorkbookDesigner لربط البيانات
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // إضافة صيغة لإظهار الإزالة
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // احسب الصيغ أولاً
            wkb.CalculateFormula();

            // إزالة جميع الصيغ من ورقة العمل
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // احفظ المصنف
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


