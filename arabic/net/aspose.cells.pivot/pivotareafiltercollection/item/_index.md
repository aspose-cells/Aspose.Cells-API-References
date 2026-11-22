---
title: "PivotAreaFilterCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotAreaFilterCollection. يحصل على الفلتر من القائمة حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.pivot/pivotareafiltercollection/item/
---
## PivotAreaFilterCollection indexer

يحصل على المرشح من القائمة حسب الفهرس.

```csharp
public PivotAreaFilter this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // إضافة جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقول إلى مناطق pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // إنشاء تنسيق شرطي
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // إنشاء منطقة محورية وإضافة عوامل التصفية
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pcf.PivotAreas.Add(pivotArea);
            
            // عرض استخدام خاصية Item
            PivotAreaFilter filter = pivotArea.Filters[0];
            filter.IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            
            // احفظ المصنف
            workbook.Save("PivotAreaFilterCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotAreaFilter](../../pivotareafilter/)
* class [PivotAreaFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


