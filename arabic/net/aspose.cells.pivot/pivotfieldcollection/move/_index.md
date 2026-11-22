---
title: "PivotFieldCollection.Move"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFieldCollection. ينقل PivotField من الموضع الحالي إلى الموضع الوجهة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldcollection/move/
---
## PivotFieldCollection.Move method

ينقل PivotField من الموضع الحالي إلى الموضع الوجهة

```csharp
public void Move(int currPos, int destPos)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| currPos | Int32 | الموضع الحالي لـ PivotField بناءً على الصفر |
| destPos | Int32 | الموضع الهدف لحقل PivotField بناءً على الصفر |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إنشاء بيانات نموذجية
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة حقول إلى منطقة الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            
            Console.WriteLine("Before move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
            
            // انقل الحقل الأول إلى الموضع 1
            pivotTable.RowFields.Move(0, 1);
            
            Console.WriteLine("\nAfter move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


