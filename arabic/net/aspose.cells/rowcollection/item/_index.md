---
title: "RowCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RowCollection. تحصل على كائن Row وفقًا لمؤشر الصف المعطى. سيتم إنشاء كائن Row للمؤشر المعطى إذا لم يكن موجودًا مسبقًا."
type: docs
url: /ar/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

يحصل على كائن [`Row`](../../row/) وفقًا لمؤشر الصف المعطى. سيتم إنشاء كائن Row للمؤشر المعطى إذا لم يكن موجودًا مسبقًا.

```csharp
public Row this[int rowIndex] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين العرض القياسي للأعمدة
            cells.StandardWidth = 20.0;

            // الوصول إلى الصفوف وتنسيقها باستخدام خاصية Item
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // الوصول إلى الخلية في الصف وتنسيقها
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // احفظ المصنف
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


