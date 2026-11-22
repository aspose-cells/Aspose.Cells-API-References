---
title: "PivotFilterCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFilterCollection. تحصل على كائن pivotfilter عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfiltercollection/item/
---
## PivotFilterCollection indexer

يحصل على كائن pivotfilter في الفهرس المحدد.

```csharp
public PivotFilter this[int index] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة مرشح محور باستخدام طريقة PivotFilterCollection.Add
            pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[0]; // Using Item property via index
            filter.Name = "SampleFilter";
            filter.Value1 = "100";
            
            // الوصول إلى المرشح باستخدام خاصية Item وعرض المعلومات
            Console.WriteLine("Filter Name: " + pivotTable.PivotFilters[0].Name);
            Console.WriteLine("Filter Value1: " + pivotTable.PivotFilters[0].Value1);
            Console.WriteLine("Filter Type: " + pivotTable.PivotFilters[0].FilterType);
            
            // احفظ المصنف
            workbook.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../../pivotfilter/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


