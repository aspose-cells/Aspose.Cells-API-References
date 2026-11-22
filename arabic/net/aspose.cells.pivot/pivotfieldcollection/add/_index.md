---
title: "PivotFieldCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFieldCollection. تضيف كائن PivotField إلى نوع PivotFields المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

يضيف كائن PivotField إلى النوع المحدد PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotField | PivotField | كائن PivotField. |

### قيمة الإرجاع

فهرس كائن PivotField في هذه PivotFields.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            
            // إضافة حقل بيانات إلى منطقة حقول الأعمدة باستخدام طريقة Add
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // حساب بيانات جدول المحور
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


