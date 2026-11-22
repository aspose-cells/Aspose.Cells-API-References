---
title: "PivotTable.RefreshedByWho"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُعيد اسم آخر مستخدم قام بتحديث هذا PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/refreshedbywho/
---
## PivotTable.RefreshedByWho property

يحصل على اسم آخر مستخدم قام بتحديث جدول المحور هذا

```csharp
public string RefreshedByWho { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshedByWhoDemo
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

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[pivotIndex];
            
            // إضافة حقول إلى جدول محوري
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.AddFieldToArea(PivotFieldType.Data, 1);
            
            // قم بتحديث جدول المحور لتعيين خاصية RefreshedByWho
            pt.RefreshData();
            pt.CalculateData();

            // إخراج معلومات التحديث
            Console.WriteLine("Pivot Table Refresh Information:");
            Console.WriteLine("Last Refresh Date: " + pt.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
            
            // احفظ وأعد التحميل لإظهار استمرارية الخاصية
            string savePath = "PivotTableRefreshedByWhoDemo_Out.xlsx";
            wb.Save(savePath);
            
            // أعد تحميل المصنف وتحقق من الخاصية
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter Reload:");
            Console.WriteLine("Last Refresh Date: " + pt2.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt2.RefreshedByWho);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


