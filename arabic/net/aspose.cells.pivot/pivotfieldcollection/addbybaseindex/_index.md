---
title: "PivotFieldCollection.AddByBaseIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFieldCollection. تضيف كائن PivotField إلى نوع PivotFields المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldcollection/addbybaseindex/
---
## PivotFieldCollection.AddByBaseIndex method

يضيف كائن PivotField إلى النوع المحدد PivotFields.

```csharp
public int AddByBaseIndex(int baseFieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| baseFieldIndex | Int32 | فهرس الحقل في PivotFields الأساسية. |

### قيمة الإرجاع

فهرس كائن PivotField في هذه PivotFields.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddByBaseIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Year";
            worksheet.Cells["B2"].Value = 2022;
            worksheet.Cells["B3"].Value = 2023;
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C3", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // إضافة الحقول الأولية
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // إضافة حقل السنة إلى منطقة الصف باستخدام AddByBaseIndex
            int newIndex = pivotTable.RowFields.AddByBaseIndex(1);
            Console.WriteLine("Added field at index: " + newIndex);

            workbook.Save("PivotFieldAddByBaseIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


