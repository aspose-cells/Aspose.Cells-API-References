---
title: "PivotTable.RowRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُرجِع كائن CellArea يمثل النطاق الذي يحتوي على منطقة الصف في تقرير PivotTable. للقراءة فقط"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

يرجع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة الصف في تقرير جدول المحور. للقراءة فقط.

```csharp
public CellArea RowRange { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // امسح جميع جداول المحور من دفتر العمل
            workbook.Worksheets.RefreshAll();
            
            // احصل على أول جدول محوري من أول ورقة عمل
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // احصل على نطاق الصف للجدول المحوري
            CellArea rowRange = pivotTable.RowRange;
            
            // اعرض إحداثيات نطاق الصف
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // احصل على نطاق العمود للجدول المحوري
            CellArea columnRange = pivotTable.ColumnRange;
            
            // اعرض إحداثيات نطاق العمود
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


