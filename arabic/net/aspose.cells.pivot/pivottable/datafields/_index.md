---
title: "PivotTable.DataFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُعيد PivotFieldCollection التي تمثل جميع حقول البيانات في PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

تُعيد [`PivotFieldCollection`](../../pivotfieldcollection/) التي تمثل جميع حقول البيانات في PivotTable.

```csharp
public PivotFieldCollection DataFields { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldsDemo
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

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // الوصول إلى حقول البيانات وإظهار الوظيفة
            PivotFieldCollection dataFields = pivotTable.DataFields;
            if (dataFields.Count > 0)
            {
                PivotField dataField = dataFields[0];
                Console.WriteLine("Data Field Name: " + dataField.Name);
                Console.WriteLine("Data Field Function: " + dataField.Function);
            }

            // احفظ المصنف
            workbook.Save("PivotTableDataFieldsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


