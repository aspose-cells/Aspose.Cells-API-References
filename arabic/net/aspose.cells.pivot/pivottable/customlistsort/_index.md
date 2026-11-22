---
title: "PivotTable.CustomListSort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان يجب اعتبار القائمة المخصصة المدمجة عند فرز البيانات"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/customlistsort/
---
## PivotTable.CustomListSort property

يشير إلى ما إذا كان يجب أخذ القائمة المخصصة المدمجة في الاعتبار عند فرز البيانات

```csharp
public bool CustomListSort { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyCustomListSortDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Pear";
            cells["B5"].Value = 5;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // تمكين فرز القوائم المخصصة
            pivotTable.CustomListSort = true;

            // احفظ المصنف
            workbook.Save("PivotTable_CustomListSort_Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


