---
title: "DataSorterKey.IconId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorterKey. تمثّل معرف نوع مجموعة الأيقونات"
type: docs
url: /ar/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

يمثل المعرف لنوع مجموعة الأيقونات.

```csharp
public int IconId { get; }
```

### ملاحظات

يعمل فقط عندما يكون [`Type`](../type/) هو Icon.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تجريبية بقيم يمكن أن تستخدم مجموعات الأيقونات
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

            // إنشاء مُرتّب البيانات وإضافة المفتاح
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // فرز البيانات
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // عرض خاصية IconId من مفاتيح المُرتّب
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // احفظ المصنف
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
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

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


