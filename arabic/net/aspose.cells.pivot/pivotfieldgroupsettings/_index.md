---
title: "الفئة PivotFieldGroupSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotFieldGroupSettings. تمثل إعداد مجموعة حقل pivot"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldgroupsettings/
---
## PivotFieldGroupSettings class

يمثل إعداد مجموعة حقل محوري.

```csharp
public class PivotFieldGroupSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PivotFieldGroupSettings](pivotfieldgroupsettings/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [Type](../../aspose.cells.pivot/pivotfieldgroupsettings/type/) { get; } | يحصل على نوع المجموعة لحقل pivot. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsDemo
    {
        public static void PivotFieldGroupSettingsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Amount";
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // أضف جدولًا محوريًا إلى ورقة العمل
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // الوصول إلى حقل الصف
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);

            // الوصول إلى إعدادات المجموعة لحقل الصف
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // عرض نوع المجموعة لحقل pivot
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // احفظ المصنف
            workbook.Save("PivotFieldGroupSettingsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


