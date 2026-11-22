---
title: "PivotField.FilterByLabel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. يصفى حسب عناوين الحقول المحورية للصف أو العمود"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

تصفية حسب التسميات لحقل pivot للصف أو العمود.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | PivotFilterType | نوع بيانات الفلترة. |
| label1 | String | تسمية شرط الفلتر |
| label2 | String | التسمية العليا لشرط الفلتر بين |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // إنشاء جدول محوري باستخدام المعلمات الصحيحة
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // احصل على حقل Pivot
            PivotField field = pivot.RowFields[0];
            
            // تطبيق الفلاتر
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotFilterByLabelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


