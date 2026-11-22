---
title: "CellArea.StartColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "حقل CellArea. يحصل أو يضبط العمود الابتدائي لهذه المنطقة."
type: docs
url: /ar/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

يحصل أو يضبط العمود الابتدائي لهذه المساحة.

```csharp
public int StartColumn;
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ضبط بعض البيانات الأولية.
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // إنشاء CellArea وضبط العمود الابتدائي الخاص به.
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // إدراج عمود جديد عن طريق إزاحة الخلايا الموجودة إلى الأسفل.
            cells.InsertRange(area, ShiftType.Down);

            // تحقق من النتيجة
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


