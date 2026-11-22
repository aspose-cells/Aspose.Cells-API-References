---
title: "الفئة PivotTableRefreshOption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotTableRefreshOption. تمثل خيارات تحديث مصدر بيانات جدول pivot"
type: docs
url: /ar/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

يمثل خيارات تحديث مصدر بيانات جدول محوري.

```csharp
public class PivotTableRefreshOption
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | يمثل خيارات تحديث مصدر بيانات جدول محوري. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | يشير إلى ما إذا كان يجب الحفاظ على الترتيب الأصلي لعناصر pivot كما في مصدر البيانات القديم. |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | يشير إلى ما إذا كان يجب الحفاظ على بيانات المجموعة المحلية المخزنة مؤقتًا إذا ظلت القيم القصوى والدنيا دون تغيير. القيمة الافتراضية هي false مما يعني تحديث المجموعة بالإعداد المحلي. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | تمثل طريقة حجز العناصر المفقودة في pivot. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // أضف جدولًا محوريًا إلى ورقة العمل
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // إنشاء نسخة من PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // تحديث جدول pivot باستخدام الخيارات المحددة
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


