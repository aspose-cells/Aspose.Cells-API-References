---
title: "PivotField.Number"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تمثل تنسيق العرض المدمج للأرقام والتواريخ"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

يمثل تنسيق العرض المدمج للأرقام والتواريخ.

```csharp
public int Number { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNumberDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
            sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
            sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
            
            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // أضف حقل تاريخ إلى منطقة الأعمدة واضبط تنسيق الأرقام
            int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField field = pivot.ColumnFields[fieldIndex];
            field.Number = 16; // d-mmm format
            
            // تحديث وحساب الجدول المحوري
            pivot.RefreshData();
            pivot.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotFieldNumberDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


