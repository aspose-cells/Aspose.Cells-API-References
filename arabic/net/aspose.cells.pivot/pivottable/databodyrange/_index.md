---
title: "PivotTable.DataBodyRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُرجع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة البيانات في القائمة بين صف الرأس وصف الإدراج. للقراءة فقط"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

يرجع كائن [`CellArea`](../../../aspose.cells/cellarea/) الذي يمثل النطاق الذي يحتوي على منطقة البيانات في القائمة بين صف الرأس وصف الإدراج. للقراءة فقط.

```csharp
public CellArea DataBodyRange { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // إضافة بيانات عينة لجدول محوري
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // إضافة جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // تكوين جدول محوري
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تحديث بيانات جدول المحور
            pivot.RefreshData();
            pivot.CalculateData();

            // توضيح استخدام DataBodyRange
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // احفظ المصنف
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


