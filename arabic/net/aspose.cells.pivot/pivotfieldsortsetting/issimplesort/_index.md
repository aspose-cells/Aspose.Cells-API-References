---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFieldSortSetting. تشير إلى ما إذا كان سيتم تطبيق عملية فرز بيانات بسيطة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

يشير إلى ما إذا كان سيتم تطبيق عملية فرز بيانات بسيطة.

```csharp
public bool IsSimpleSort { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احصل على حقل المحور
            PivotField pivotField = pivotTable.RowFields[0];

            // احصل على إعداد الفرز (خاصية للقراءة فقط)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // اعرض قيمة IsSimpleSort الحالية
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // ملاحظة: IsSimpleSort للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // للتوضيح كيفية الفرز، سننشئ جدولًا محوريًا جديدًا بفرز مختلف

            // أنشئ جدولًا محوريًا آخر بفرز مخصص
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // قم بفرز حقل المحور باستخدام الطريقة المتاحة
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // احفظ المصنف
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


