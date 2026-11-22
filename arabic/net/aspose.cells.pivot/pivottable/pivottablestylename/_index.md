---
title: "PivotTable.PivotTableStyleName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل أو تعين اسم النمط لجدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/pivottablestylename/
---
## PivotTable.PivotTableStyleName property

يحصل أو يضبط اسم النمط لجدول المحور.

```csharp
public string PivotTableStyleName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Data;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء بيانات نموذجية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // تطبيق نمط جدول محوري مدمج
            pivotTable.PivotTableStyleName = "PivotStyleLight16";
            
            // احفظ المصنف
            workbook.Save("PivotTableStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


