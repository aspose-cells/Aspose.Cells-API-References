---
title: "FindOptions.SetRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FindOptions. تحدد النطاق الذي يتم البحث فيه"
type: docs
url: /ar/net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

يضبط النطاق الذي تم البحث فيه.

```csharp
public void SetRange(CellArea ca)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | النطاق الذي يتم البحث فيه. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsMethodSetRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بعض البيانات
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("def");
            worksheet.Cells["C3"].PutValue("abc");
            
            // أنشئ FindOptions وحدد نطاق البحث
            FindOptions rangeOptions = new FindOptions();
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 1;
            cellarea.StartColumn = 1;
            cellarea.EndRow = 3;
            cellarea.EndColumn = 3;
            rangeOptions.SetRange(cellarea);
            
            // ابحث داخل النطاق المحدد
            rangeOptions.SearchBackward = false;
            Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
            
            Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


