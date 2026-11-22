---
title: "PivotFilter.Value1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFilter. يحصل على قيمة السلسلة value1 لفلتر المحور الملصق"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfilter/value1/
---
## PivotFilter.Value1 property

يحصل على القيمة النصية 1 للملصق في مرشح المحور.

```csharp
public string Value1 { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValue1Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // ملء ورقة العمل ببيانات عينة
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // إضافة جدول محوري
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // أضف فلتر محور واضبط Value1
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Value1 = "Apple"; // Filter for Apple products only

            // تحديث وحساب البيانات
            pivot.RefreshData();
            pivot.CalculateData();

            // احفظ المصنف
            book.Save("PivotFilterValue1Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


