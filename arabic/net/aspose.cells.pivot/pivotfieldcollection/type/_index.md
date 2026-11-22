---
title: "PivotFieldCollection.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFieldCollection. يحصل على نوع PivotFields"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldcollection/type/
---
## PivotFieldCollection.Type property

يحصل على نوع PivotFields.

```csharp
public PivotFieldType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // عرض نوع مجموعة حقول pivot
            Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);

            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotFieldCollection dataFields = pivotTable.DataFields;

            // عرض نوع مجموعة حقول البيانات
            Console.WriteLine("DataFields Type: " + dataFields.Type);

            // احسب البيانات وقم بتحديث جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // حفظ النتيجة
            workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


