---
title: "PivotTable.ShowInTabularForm"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تنسق PivotTable في شكل جدولي"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showintabularform/
---
## PivotTable.ShowInTabularForm method

يصمم PivotTable في شكل جدولي.

```csharp
public void ShowInTabularForm()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInTabularFormDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل البيانات
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // إضافة بيانات عينة لجدول محوري
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // إضافة ورقة جدول Pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // إضافة جدول محوري
            int pivotIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // إضافة حقول إلى جدول محوري
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // عرض جدول Pivot في شكل جدولي
            pivotTable.ShowInTabularForm();
            
            // تحديث وحساب بيانات جدول البيفوت
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTableShowInTabularFormDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


