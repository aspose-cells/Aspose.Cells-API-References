---
title: "PivotTable.EnableWizard"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان معالج PivotTable متاحًا"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/enablewizard/
---
## PivotTable.EnableWizard property

يشير إلى ما إذا كان معالج PivotTable متاحًا.

```csharp
public bool EnableWizard { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableWizardDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 2000;

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // تعطيل معالج جدول المحور
            pivotTable.EnableWizard = false;

            // احفظ المصنف
            workbook.Save("PivotTable_EnableWizard_Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


