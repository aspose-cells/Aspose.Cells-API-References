---
title: "PivotDiscreteGroupSettings.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotDiscreteGroupSettings. تحصل على نوع المجموعة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotdiscretegroupsettings/type/
---
## PivotDiscreteGroupSettings.Type property

يحصل على نوع المجموعة.

```csharp
public override PivotFieldGroupType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDiscreteGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // تجميع العناصر
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { 
                new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }) 
            }, true);

            // احصل على إعدادات المجموعة ووضح خاصية Type
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);

            workbook.Save("PivotDiscreteGroupSettingsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


