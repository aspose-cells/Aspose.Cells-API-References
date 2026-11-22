---
title: "PivotTable.ShowReportFilterPageByName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. إظهار جميع صفحات مرشح التقرير وفقًا لاسم PivotFields؛ يجب أن يكون PivotField موجودًا في PageFields"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showreportfilterpagebyname/
---
## PivotTable.ShowReportFilterPageByName method

اعرض جميع صفحات مرشح التقرير وفقًا لاسم PivotField، يجب أن يكون PivotField موجودًا في PageFields.

```csharp
public void ShowReportFilterPageByName(string fieldName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldName | String | اسم PivotField |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            
            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // إضافة حقل صفحة
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Fruit");
            pivotTable.PageFields[0].Name = "FruitFilter";
            
            // تحديث جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // إظهار صفحات مرشح التقرير حسب الاسم
            pivotTable.ShowReportFilterPageByName("FruitFilter");
            
            // احفظ المصنف
            workbook.Save("PivotTableShowReportFilterPageByNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


