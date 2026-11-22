---
title: "ColumnCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ColumnCollection. يحصل على كائن Column حسب فهرس العمود. سيتم إنشاء كائن Column للفهرس المحدد إذا لم يكن موجودًا مسبقًا"
type: docs
url: /ar/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

يحصل على كائن [`Column`](../../column/) حسب فهرس العمود. سيتم إنشاء كائن Column للفهرس المحدد إذا لم يكن موجودًا مسبقًا.

```csharp
public Column this[int columnIndex] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مجموعة الأعمدة
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // حدد عرض الأعمدة باستخدام خاصية Item
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // عرض عرض الأعمدة
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // تحقق من ضبط عرض الأعمدة بشكل صحيح
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### انظر أيضًا

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


