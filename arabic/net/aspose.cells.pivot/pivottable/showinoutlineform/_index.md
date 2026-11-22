---
title: "PivotTable.ShowInOutlineForm"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تُنسق PivotTable في شكل مخطط"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showinoutlineform/
---
## PivotTable.ShowInOutlineForm method

يصمم PivotTable في شكل مخطط.

```csharp
public void ShowInOutlineForm()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInOutlineFormDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل بيانات عينة
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // أضف بيانات تجريبية
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["B1"].PutValue("Product");
            dataSheet.Cells["C1"].PutValue("Sales");
            
            dataSheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            dataSheet.Cells["B2"].PutValue("Apple");
            dataSheet.Cells["C2"].PutValue(1000);
            
            dataSheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
            dataSheet.Cells["B3"].PutValue("Banana");
            dataSheet.Cells["C3"].PutValue(2000);
            
            dataSheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
            dataSheet.Cells["B4"].PutValue("Apple");
            dataSheet.Cells["C4"].PutValue(1500);
            
            // إنشاء ورقة عمل جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // إضافة جدول محوري والحصول على المرجع
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C4", 
                "A3", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
                
            // إضافة حقول إلى المناطق
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // إظهار في شكل مخطط
            pivotTable.ShowInOutlineForm();
            
            // تحديث وحساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTableOutlineFormDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


