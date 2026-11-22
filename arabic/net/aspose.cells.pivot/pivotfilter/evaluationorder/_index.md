---
title: "PivotFilter.EvaluationOrder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFilter. تحصل على ترتيب التقييم لمرشح المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/evaluationorder/
---
## PivotFilter.EvaluationOrder property

يحصل على ترتيب التقييم لمرشح المحور.

```csharp
public int EvaluationOrder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyEvaluationOrderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء بيانات عينة
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // إنشاء جدول محوري
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivots[pivotIndex];
            
            // إضافة حقول
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // إضافة مرشح محوري
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            
            // تعيين خصائص المرشح بما في ذلك EvaluationOrder
            filter.EvaluationOrder = 1;
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // تحديث جدول المحور
            pivot.RefreshData();
            pivot.CalculateData();

            // احفظ دفتر العمل
            book.Save("PivotFilterEvaluationOrderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


