---
title: "PivotTable.MergeLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. يحصل أو يضبط ما إذا كان يجب دمج تسميات الحقول الصفية/العمودية التي تمتد عبر خلايا متعددة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/mergelabels/
---
## PivotTable.MergeLabels property

يحصل أو يضبط ما إذا كان يجب دمج تسميات حقول الصف/العمود التي تمتد عبر خلايا متعددة.

```csharp
public bool MergeLabels { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMergeLabelsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Apple";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Orange";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // تمكين دمج التسميات
            pivotTable.MergeLabels = true;
            
            // احفظ المصنف
            workbook.Save("PivotTableMergeLabelsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


