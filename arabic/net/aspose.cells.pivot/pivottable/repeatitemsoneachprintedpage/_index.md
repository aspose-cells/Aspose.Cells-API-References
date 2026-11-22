---
title: "PivotTable.RepeatItemsOnEachPrintedPage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كانت عناوين عنصر المحور في منطقة الصف تُكرر في كل صفحة مطبوعة لحقول المحور في الشكل الجدولي"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/
---
## PivotTable.RepeatItemsOnEachPrintedPage property

يشير إلى ما إذا كانت تسميات عنصر المحور في منطقة الصف تُكرر في كل صفحة مطبوعة لحقول المحور في الشكل الجدولي.

```csharp
public bool RepeatItemsOnEachPrintedPage { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRepeatItemsOnEachPrintedPageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("North");
            worksheet.Cells["A4"].PutValue("South");
            worksheet.Cells["A5"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Apples");
            worksheet.Cells["B3"].PutValue("Oranges");
            worksheet.Cells["B4"].PutValue("Apples");
            worksheet.Cells["B5"].PutValue("Oranges");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["C5"].PutValue(2500);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تعيين إعداد الصفحة للطباعة
            worksheet.PageSetup.PrintTitleRows = "$1:$1";
            worksheet.PageSetup.PrintArea = "A1:G20";
            worksheet.PageSetup.FitToPagesTall = 0;
            worksheet.PageSetup.FitToPagesWide = 1;

            // عرض القيمة الحالية لـ RepeatItemsOnEachPrintedPage
            Console.WriteLine("Current RepeatItemsOnEachPrintedPage value: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // تمكين تكرار العناصر في كل صفحة مطبوعة
            pivotTable.RepeatItemsOnEachPrintedPage = true;
            Console.WriteLine("RepeatItemsOnEachPrintedPage set to: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // احسب البيانات لملء جدول المحور
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotTableRepeatItemsOnEachPrintedPageDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


