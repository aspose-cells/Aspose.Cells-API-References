---
title: "PivotPageFields.PivotPageFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ PivotPageFields. يمثل عناصر حقل صفحة المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

تمثل عناصر حقل صفحة pivot.

```csharp
public PivotPageFields()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // أنشئ حقول صفحة المحور باستخدام المنشئ
            PivotPageFields pageFields = new PivotPageFields();
            
            // أضف حقول الصفحة
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // أضف التعريف
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // أضف جدول محوري مع المعلمات الصحيحة
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // احفظ المصنف
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


