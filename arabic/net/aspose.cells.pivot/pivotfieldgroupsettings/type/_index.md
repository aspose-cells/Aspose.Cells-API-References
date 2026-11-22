---
title: "PivotFieldGroupSettings.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFieldGroupSettings. تحصل على نوع المجموعة لحقل المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldgroupsettings/type/
---
## PivotFieldGroupSettings.Type property

يحصل على نوع المجموعة لحقل pivot.

```csharp
public virtual PivotFieldGroupType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            worksheet.Cells["A3"].Value = new DateTime(2023, 1, 2);
            worksheet.Cells["A4"].Value = new DateTime(2023, 1, 3);

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // أضف جدولًا محوريًا إلى ورقة العمل
                int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "D3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // إضافة حقول إلى الجدول المحوري
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

                // الوصول إلى حقل الصف وتجميعه حسب التاريخ
                PivotField rowField = pivotTable.RowFields[0];
                rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("DateGroup", new int[] { 0, 1 }) }, true);

                // الوصول إلى إعدادات المجموعة لحقل الصف
                PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

                // عرض القيمة الحالية لخاصية Type (للقراءة فقط)
                Console.WriteLine("Pivot Field Group Type: " + groupSettings.Type);

                // احفظ المصنف
                workbook.Save("PivotFieldGroupSettingsTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotFieldGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


