---
title: "التعداد PivotFieldDataDisplayFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Pivot.PivotFieldDataDisplayFormat. يمثل تنسيق عرض البيانات في حقل بيانات PivotTable."
type: docs
url: /ar/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

يمثل تنسيق عرض البيانات في حقل البيانات لجدول PivotTable.

```csharp
public enum PivotFieldDataDisplayFormat
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Normal | `0` | يمثل تنسيق العرض العادي. |
| DifferenceFrom | `1` | يمثل الفرق عن تنسيق العرض. |
| PercentageOf | `2` | يمثل النسبة المئوية لتنسيق العرض. |
| PercentageDifferenceFrom | `3` | يمثل الفرق النسبي عن تنسيق العرض. |
| RunningTotalIn | `4` | يمثل الإجمالي المتراكم في تنسيق العرض. |
| PercentageOfRow | `5` | يمثل النسبة المئوية لتنسيق عرض الصف. |
| PercentageOfColumn | `6` | يمثل النسبة المئوية لتنسيق عرض العمود. |
| PercentageOfTotal | `7` | يمثل النسبة المئوية لتنسيق العرض الكلي. |
| Index | `8` | يمثل تنسيق عرض الفهرس. |
| PercentageOfParentRowTotal | `9` | يمثل النسبة المئوية لتنسيق إجمالي صف الأصل. |
| PercentageOfParentColumnTotal | `10` | يمثل النسبة المئوية لتنسيق إجمالي عمود الأصل. |
| PercentageOfParentTotal | `11` | يمثل النسبة المئوية لتنسيق إجمالي الأصل. |
| PercentageOfRunningTotalIn | `12` | يمثل النسبة المئوية للإجمالي المتراكم في تنسيق العرض. |
| RankSmallestToLargest | `13` | يمثل تنسيق العرض من الأصغر إلى الأكبر. |
| RankLargestToSmallest | `14` | يمثل تنسيق العرض من الأكبر إلى الأصغر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDataDisplayFormatDemo
    {
        public static void PivotFieldDataDisplayFormatExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // أضف بعض البيانات التجريبية
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // إضافة جدول محوري
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // تعيين نمط جدول المحور
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // تغيير سمات PivotField
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // تعيين DataDisplayFormat
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // تحديث وحساب البيانات
            pivot.RefreshData();
            pivot.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


