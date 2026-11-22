---
title: "PivotTable.AltTextDescription"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على وصف النص البديل"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/alttextdescription/
---
## PivotTable.AltTextDescription property

يحصل على وصف النص البديل.

```csharp
public string AltTextDescription { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextDescriptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // عرض الوصف النصي البديل الحالي
            Console.WriteLine("Current AltTextDescription: " + pivotTable.AltTextDescription);

            // تعيين وصف نص بديل جديد
            pivotTable.AltTextDescription = "Sales data by product category";

            // احفظ المصنف
            workbook.Save("PivotTableAltTextDescriptionDemo.xlsx");

            // عرض الوصف النصي البديل الجديد
            Console.WriteLine("New AltTextDescription: " + pivotTable.AltTextDescription);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


