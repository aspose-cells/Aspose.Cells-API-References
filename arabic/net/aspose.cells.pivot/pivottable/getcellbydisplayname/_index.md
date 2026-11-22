---
title: "PivotTable.GetCellByDisplayName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تحصل على كائن Cell بواسطة اسم العرض لـ PivotField"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

يحصل على كائن [`Cell`](../../../aspose.cells/cell/) بواسطة اسم العرض لـ PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| displayName | String | اسم DisplayName لـ PivotField |

### قيمة الإرجاع

كائن Cell

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetCellByDisplayNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احصل على اسم عرض حقل البيانات
            string displayName = pivotTable.DataFields[0].DisplayName;

            // استخدم طريقة GetCellByDisplayName
            Cell cell = pivotTable.GetCellByDisplayName(displayName);

            // إخراج النتائج
            Console.WriteLine("Display Name: " + displayName);
            Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
            Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));

            // احفظ المصنف
            workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


