---
title: "Enum SlicerStyleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Slicers.SlicerStyleType. حدد نمط عرض المحدد"
type: docs
url: /ar/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

حدد نمط عرض المقطّع.

```csharp
public enum SlicerStyleType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | النمط الفاتح المدمج الأول |
| SlicerStyleLight2 | `1` | النمط الفاتح المدمج الثاني |
| SlicerStyleLight3 | `2` | النمط الفاتح المدمج الثالث |
| SlicerStyleLight4 | `3` | النمط الفاتح المدمج الرابع |
| SlicerStyleLight5 | `4` | النمط الفاتح المدمج الخامس |
| SlicerStyleLight6 | `5` | النمط الفاتح المدمج السادس |
| SlicerStyleOther1 | `6` | النمط المدمج الآخر الأول |
| SlicerStyleOther2 | `7` | النمط المدمج الآخر الثاني |
| SlicerStyleDark1 | `8` | النمط الداكن المدمج الأول |
| SlicerStyleDark2 | `9` | النمط الداكن المدمج الثاني |
| SlicerStyleDark3 | `10` | النمط الداكن المدمج الثالث |
| SlicerStyleDark4 | `11` | النمط الداكن المدمج الرابع |
| SlicerStyleDark5 | `12` | النمط الداكن المدمج الخامس |
| SlicerStyleDark6 | `13` | النمط الداكن المدمج السادس |
| Custom | `14` | نمط معرف من قبل المستخدم، غير مدعوم حالياً |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة مقطع
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // تعيين نمط المقطّع
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // احفظ المصنف
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


