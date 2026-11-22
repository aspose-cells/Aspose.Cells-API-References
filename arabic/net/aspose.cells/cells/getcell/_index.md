---
title: "Cells.GetCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على عنصر Cell أو null في مؤشر صف الخلية المحدد ومؤشر العمود المحدد"
type: docs
url: /ar/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

يحصل على عنصر [`Cell`](../../cell/) أو null في مؤشر صف الخلية المحدد ومؤشر العمود المحدد.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف |
| عمود | Int32 | فهرس العمود |

### قيمة الإرجاع

إرجاع كائن Cell إذا كان كائن Cell موجودًا. إرجاع null إذا لم تكن الخلية موجودة.

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام طريقة CheckCell(int row, int column). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ فبراير 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية في الصف 1، العمود 2 (فهرس يبدأ من 0)
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // تعيين القيمة والنمط للعرض
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


