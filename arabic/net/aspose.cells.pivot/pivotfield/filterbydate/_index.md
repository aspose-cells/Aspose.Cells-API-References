---
title: "PivotField.FilterByDate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تقوم بتصفية القيم التاريخية لحقل المحور الصف أو العمود"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

يفلتر حسب قيم التاريخ لحقل المحور الصف أو العمود.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | PivotFilterType | نوع بيانات الفلترة. |
| dateTime1 | DateTime | تسمية التاريخ لشرط الفلتر |
| dateTime2 | DateTime | التسمية العليا للتاريخ لشرط الفلتر بين |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة مع تواريخ
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // أضف حقل التاريخ إلى منطقة العمود
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // طبق مرشح التاريخ (تواريخ سبتمبر بين 2020-2021)
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // حفظ النتائج
            workbook.Save("FilterByDateDemo.xlsx");
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


