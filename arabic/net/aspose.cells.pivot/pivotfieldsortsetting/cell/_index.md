---
title: "PivotFieldSortSetting.Cell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFieldSortSetting. يفرز حسب القيم في أي صف أو عمود"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldsortsetting/cell/
---
## PivotFieldSortSetting.Cell property

يتم الفرز حسب القيم في أي صف أو عمود.

```csharp
public string Cell { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyCellDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 5;
            cells["B4"].Value = 8;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // فرز حسب مرجع الخلية
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A2");
            
            // عرض مثال لاستخدام خاصية Cell
            Console.WriteLine("Sorting by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // تغيير خلية الفرز
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "A3");
            Console.WriteLine("Changed sort cell to: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // مسح فرز الخلايا
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            Console.WriteLine("After clearing cell sort: " + 
                (string.IsNullOrEmpty(pivotTable.RowFields[0].SortSetting.Cell) ? "Empty" : "Has value"));
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


