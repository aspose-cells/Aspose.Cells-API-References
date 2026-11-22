---
title: "PivotTable.ManualUpdate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

يشير إلى ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم.

```csharp
public bool ManualUpdate { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyManualUpdateDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet dataSheet = workbook.Worksheets["Sheet1"];
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["A4"].PutValue("A");
            dataSheet.Cells["B4"].PutValue(30);

            // إضافة جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int index = pivotSheet.PivotTables.Add("Sheet1!A1:B4", "A3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];

            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // تمكين التحديث اليدوي
            pivotTable.ManualUpdate = true;
            
            // في هذه المرحلة، لن يتم تحديث PivotTable تلقائيًا
            Console.WriteLine("Pivot table before refresh (ManualUpdate=true):");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will be empty
            
            // تحديث PivotTable يدويًا
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            Console.WriteLine("Pivot table after manual refresh:");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will show "40" (sum of category A)
            
            // احفظ المصنف
            workbook.Save("PivotTableManualUpdateDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


