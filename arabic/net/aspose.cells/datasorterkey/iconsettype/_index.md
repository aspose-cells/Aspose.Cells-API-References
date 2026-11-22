---
title: "DataSorterKey.IconSetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorterKey. تمثّل نوع مجموعة الأيقونات"
type: docs
url: /ar/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

يمثل نوع مجموعة الأيقونات.

```csharp
public IconSetType IconSetType { get; }
```

### ملاحظات

يعمل فقط عندما يكون [`Type`](../type/) هو Icon.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تجريبية مع تنسيق شرطي لمجموعة الأيقونات
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // إضافة تنسيق شرطي لمجموعة الأيقونات
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // إنشاء مُرتّب البيانات بنوع مجموعة الأيقونات
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // فرز البيانات
            sorter.Sort(worksheet.Cells, area);

            // عرض نوع مجموعة الأيقونات من مفتاح المُرتّب
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // احفظ المصنف
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


