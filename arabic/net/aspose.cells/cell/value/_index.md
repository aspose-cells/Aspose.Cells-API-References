---
title: "Cell.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل/تضبط القيمة الموجودة في هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/value/
---
## Cell.Value property

يحصل/يضبط القيمة الموجودة في هذه الخلية.

```csharp
public object Value { get; set; }
```

### ملاحظات

النوع المحتمل:

null,

Boolean,

DateTime,

Double,

Integer

String.

بالنسبة لقيمة int، قد يتم إرجاعها ككائن Integer أو ككائن Double. ولا يوجد ضمان بأن القيمة المرجعة ستظل من نفس نوع الكائن دائمًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين القيم باستخدام الخاصية Value
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // إظهار قيم null
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // عرض القيم
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


