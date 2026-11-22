---
title: "PivotTable.IsExcel2003Compatible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديثه؛ إذا كان true يجب أن يكون طول السلسلة أقل من أو يساوي 255 حرفًا، فإذا كان طول السلسلة أكبر من 255 حرفًا سيتم قطعه. إذا كان false لن تُطبق هذه القيود على السلسلة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable، إذا كانت true، يجب أن تكون السلسلة أقل من أو تساوي 255 حرفًا، لذا إذا كانت السلسلة أطول من 255 حرفًا، سيتم قطعها. إذا كانت false، لن تخضع السلسلة للقيود المذكورة أعلاه. القيمة الافتراضية هي true.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsExcel2003CompatibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet dataSheet = wb.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].Value = "Product";
            dataSheet.Cells["B1"].Value = "Description";
            dataSheet.Cells["C1"].Value = "Status";
            dataSheet.Cells["D1"].Value = "Date";
            
            // إضافة صفوف بيانات العينة
            dataSheet.Cells["A2"].Value = "Product1";
            dataSheet.Cells["B2"].Value = "Short description";
            dataSheet.Cells["C2"].Value = "Active";
            dataSheet.Cells["D2"].Value = DateTime.Now;
            
            dataSheet.Cells["A3"].Value = "Product2";
            dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
            dataSheet.Cells["C3"].Value = "Inactive";
            dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);

            // إضافة جدول محوري
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // تكوين حقول الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
            
            // تعيين وضع التوافق
            pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
            
            // تحديث وحساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


