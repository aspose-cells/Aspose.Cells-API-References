---
title: "تعداد PivotRefreshState"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Pivot.PivotRefreshState. الحالة لتحديث جداول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotrefreshstate/
---
## PivotRefreshState enumeration

الحالة لتحديث جداول pivot.

```csharp
public enum PivotRefreshState
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Success | `0` | تم التحديث بنجاح |
| UnsupportedExternalDataSource | `1` | فشل التحديث لأن مصدر البيانات خارجي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotRefreshStateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مع جدول محوري نموذجي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // عرض PivotRefreshState
            PivotRefreshState refreshState = pivotTable.RefreshData();
            if (refreshState == PivotRefreshState.Success)
            {
                Console.WriteLine("Pivot table refreshed successfully");
            }
            else if (refreshState == PivotRefreshState.UnsupportedExternalDataSource)
            {
                Console.WriteLine("External data source not supported - calculating data instead");
                pivotTable.CalculateData();
            }

            // احفظ المصنف
            workbook.Save("PivotRefreshStateDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


