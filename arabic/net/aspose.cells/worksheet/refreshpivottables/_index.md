---
title: "Worksheet.RefreshPivotTables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تقوم بتحديث جميع PivotTables في هذه Worksheet"
type: docs
url: /ar/net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

يقوم بتحديث جميع جداول Pivot في هذه ورقة العمل.

```csharp
public void RefreshPivotTables()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر الذي يحتوي على جداول Pivot
            Workbook workbook = new Workbook("example.xlsx");
            
            // احصل على أول ورقة عمل تحتوي على جداول Pivot
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تحديث جميع جداول Pivot في ورقة العمل
            worksheet.RefreshPivotTables();
            
            // حفظ المصنف المحدث
            workbook.Save("RefreshedPivotTables.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

يقوم بتحديث جميع جداول Pivot في هذه ورقة العمل.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيار | PivotTableRefreshOption | الخيار لتحديث مصدر بيانات جدول Pivot. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            worksheet.RefreshPivotTables();

            int preCount = pivotTable.RowFields[0].PivotItems.Count;


            // تعديل بيانات المصدر
            worksheet.Cells["A2"].Value = "test2";
            worksheet.Cells["A3"].Value = "test3";

            // إنشاء خيارات التحديث
            PivotTableRefreshOption options = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
            };
            worksheet.RefreshPivotTables(options);
            int nowCount = pivotTable.RowFields[0].PivotItems.Count;
            Console.WriteLine(nowCount > preCount);
                        

            // حفظ النتيجة
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


