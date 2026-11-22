---
title: "التعداد PivotLineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Pivot.PivotLineType. يحدد نوع PivotLine"
type: docs
url: /ar/net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

يحدد نوع PivotLine.

```csharp
public enum PivotLineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Regular | `0` | PivotLine عادي مع عناصر pivot. |
| Subtotal | `1` | خط المجموع الفرعي. |
| GrandTotal | `2` | سطر الإجمالي الكلي. |
| Blank | `3` | سطر فارغ بعد كل مجموعة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotLineTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // فرز حقل الصف حسب القيم بترتيب تنازلي
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
            
            // حساب بيانات جدول المحور
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotLineTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


