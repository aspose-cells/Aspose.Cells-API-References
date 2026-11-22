---
title: "PivotTable.ShowEmptyCol"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showemptycol/
---
## PivotTable.ShowEmptyCol property

يشير إلى ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول

```csharp
public bool ShowEmptyCol { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyColDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // عرض القيمة الحالية لـ ShowEmptyCol
            Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);

            // تعيين ShowEmptyCol إلى false (إخفاء الأعمدة الفارغة)
            pivotTable.ShowEmptyCol = false;
            Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");

            // حساب بيانات جدول المحور
            pivotTable.CalculateData();

            // حفظ المصنف مع الأعمدة الفارغة المخفية
            workbook.Save("PivotTableHideEmptyCols.xlsx");

            // تعيين ShowEmptyCol إلى true (إظهار الأعمدة الفارغة)
            pivotTable.ShowEmptyCol = true;
            Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");

            // إعادة حساب بيانات جدول محوري
            pivotTable.CalculateData();

            // حفظ المصنف مع الأعمدة الفارغة المرئية
            workbook.Save("PivotTableShowEmptyCols.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


