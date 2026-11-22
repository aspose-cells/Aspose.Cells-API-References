---
title: "PivotTable.RefreshDate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. يحصل على تاريخ ووقت آخر مرة تم فيها تحديث PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/refreshdate/
---
## PivotTable.RefreshDate property

يحصل على تاريخ ووقت آخر مرة تم فيها تحديث جدول المحور.

```csharp
public DateTime RefreshDate { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDateDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[index];
            
            // قم بتحديث جدول المحور لتعيين تاريخ التحديث
            pt.RefreshData();
            pt.CalculateData();

            // عرض معلومات تاريخ التحديث
            Console.WriteLine("Pivot Table Refresh Date: " + pt.RefreshDate.ToLongDateString());
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);

            // احفظ وأعد التحميل لإظهار الاستمرارية
            string savePath = "PivotTableRefreshDateDemo_Out.xlsx";
            wb.Save(savePath);
            
            // إعادة التحميل وعرض تاريخ التحديث مرة أخرى
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter reloading:");
            Console.WriteLine("Pivot Table Refresh Date: " + pt2.RefreshDate.ToLongDateString());
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


