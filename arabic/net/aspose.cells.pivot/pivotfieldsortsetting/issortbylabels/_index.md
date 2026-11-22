---
title: "PivotFieldSortSetting.IsSortByLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFieldSortSetting. تشير إلى ما إذا كان سيتم فرز الحقل بنفسه أو بحقل البيانات"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/
---
## PivotFieldSortSetting.IsSortByLabels property

يشير إلى ما إذا كان سيتم فرز الحقل بنفسه أو حقل البيانات.

```csharp
public bool IsSortByLabels { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSortByLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            var cells = worksheet.Cells;
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
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // احصل على إعداد فرز حقل المحور
            PivotField pivotField = pivotTable.RowFields[0];
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // اعرض قيمة IsSortByLabels الحالية
            Console.WriteLine("Current IsSortByLabels value: " + sortSetting.IsSortByLabels);

            // ملاحظة: IsSortByLabels للقراءة فقط، لذا لا يمكننا تعيينه مباشرة
            // بدلاً من ذلك، سنوضح معناها من خلال فحص إعدادات الفرز

            // اعرض خصائص الفرز المرتبطة
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);

            // احفظ المصنف
            workbook.Save("PivotFieldSortSettingPropertyIsSortByLabelsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


