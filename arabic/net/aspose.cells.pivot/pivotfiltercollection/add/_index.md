---
title: "PivotFilterCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotFilterCollection. تضيف كائن PivotFilter إلى النوع المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

تضيف كائن PivotFilter إلى النوع المحدد

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | فهرس PivotField |
| type | PivotFilterType | نوع PivotFilter |

### قيمة الإرجاع

فهرس كائن PivotFilter في هذه PivotFilterCollection.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طرق PivotFilterCollection.AddValueFilter()، AddTop10Filter()، AddLabelFilter() و AddDateFilter(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionMethodAddWithInt32PivotFilterTypeDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // بيانات عينة
            cells["A1"].Value = "Category";
            cells["A2"].Value = "A";
            cells["A3"].Value = "B";
            cells["A4"].Value = "A";
            cells["A5"].Value = "B";
            
            cells["B1"].Value = "Value";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;
            cells["B5"].Value = 40;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");

            // إضافة مرشح محوري
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            pivot.RefreshData();
            pivot.CalculateData();

            book.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


