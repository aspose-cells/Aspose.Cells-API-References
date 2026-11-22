---
title: "PivotArea.OnlyData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تشير إلى ما إذا كانت قيم البيانات فقط في منطقة البيانات للعرض عند اختيار عنصر ما يتم اختيارها ولا تشمل تسميات العنصر"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/onlydata/
---
## PivotArea.OnlyData property

يشير إلى ما إذا كانت قيم البيانات فقط (في منطقة البيانات في العرض) لتحديد عنصر ما مختارة ولا تشمل تسميات العنصر.

```csharp
public bool OnlyData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Food");
            
            worksheet.Cells["B1"].PutValue("Revenue");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(2000);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // تكوين منطقة Pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true; // Key property demonstration
            pivotArea.IsRowGrandIncluded = false;

            // تكوين الإخراج
            Console.WriteLine("OnlyData property is set to: " + pivotArea.OnlyData);
            
            workbook.Save("PivotAreaOnlyDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


