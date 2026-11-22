---
title: "فئة RowCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.RowCollection. تجمع كائنات Row التي تمثل الصفوف الفردية في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/rowcollection/
---
## RowCollection class

تجمع كائنات [`Row`](../row/) التي تمثل الصفوف الفردية في ورقة العمل.

```csharp
public class RowCollection : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | يحصل على عدد الصفوف في هذه المجموعة. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | يحصل على كائن [`Row`](../row/) وفقًا لمؤشر الصف المعطى. سيتم إنشاء كائن Row للمؤشر المعطى إذا لم يكن موجودًا مسبقًا. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | امسح جميع الصفوف والخلايا. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | يحصل على مُعدِّد يتنقل عبر الصفوف في هذه المجموعة |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | يحصل على مُعدِّد يتنقل عبر الصفوف في هذه المجموعة |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | يحصل على كائن الصف وفقًا للموقع في القائمة. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | أزل عنصر الصف في الفهرس (الموقع) المحدد في هذه المجموعة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // احصل على مجموعة الصفوف
            RowCollection rows = worksheet.Cells.Rows;

            // احصل على عدد الصفوف في المجموعة
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // احصل على الصف الأول
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // تجول عبر الصفوف باستخدام GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // احصل على صف وفقًا للفهرس
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // امسح جميع الصفوف والخلايا
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // احفظ المصنف
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


