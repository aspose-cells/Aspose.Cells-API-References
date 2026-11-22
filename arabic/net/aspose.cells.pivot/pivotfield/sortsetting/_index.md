---
title: "PivotField.SortSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تحصل على جميع إعدادات الفرز التلقائي"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/sortsetting/
---
## PivotField.SortSetting property

يحصل على جميع إعدادات الفرز التلقائي

```csharp
public PivotFieldSortSetting SortSetting { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertySortSettingDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 75;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];

            // عرض خاصية SortSetting
            rowField.SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + rowField.SortSetting.Cell);
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);

            // تغيير إعدادات الفرز
            rowField.SortBy(SortOrder.Descending, 0, PivotLineType.GrandTotal, null);
            Console.WriteLine("\nAfter changing sort settings:");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + (string.IsNullOrEmpty(rowField.SortSetting.Cell) ? "null" : rowField.SortSetting.Cell));
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldSortSetting](../../pivotfieldsortsetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


