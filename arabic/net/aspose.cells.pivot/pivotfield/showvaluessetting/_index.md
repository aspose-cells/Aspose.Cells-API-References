---
title: "PivotField.ShowValuesSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. يحصل على إعدادات عرض القيم كما عندما يكون حساب ShowDataAs قيد الاستخدام"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

يحصل على إعدادات عرض القيم كما عندما يكون حساب ShowDataAs قيد الاستخدام.

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowValuesSettingDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 1500;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 2500;
            cells["A7"].Value = "Banana";
            cells["B7"].Value = 3500;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B7", "C10", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // قم بتكوين ShowValuesSetting لعرضه كنسبة مئوية من الإجمالي
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            
            // احسب وقم بتحديث جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotFieldShowValuesSettingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


