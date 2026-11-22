---
title: "PivotField.AddCalculatedItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. أضف عنصر صيغة محسوبة إلى الحقل المحوري."
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/addcalculateditem/
---
## PivotField.AddCalculatedItem method

أضف عنصر صيغة محسوبة إلى الحقل المحوري.

```csharp
public void AddCalculatedItem(string name, string formula)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم العنصر. |
| صيغة | String | صيغة العنصر المحوري. |

### ملاحظات

يدعم فقط إضافة عنصر محسوب إلى حقل الصف/العمود.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodAddCalculatedItemWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "grape";
            sheet.Cells["A3"].Value = "kiwi";
            sheet.Cells["A4"].Value = "grape";
            sheet.Cells["A5"].Value = "kiwi";
            
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 50;
            sheet.Cells["B3"].Value = 70;
            sheet.Cells["B4"].Value = 30;
            sheet.Cells["B5"].Value = 20;

            // إنشاء جدول محوري باستخدام المعلمات الصحيحة
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // احصل على الحقل المحوري وأضف عنصرًا محسوبًا.
            PivotField fruitField = pivotTable.RowFields[0];
            fruitField.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
            
            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotFieldAddCalculatedItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


