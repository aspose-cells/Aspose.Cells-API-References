---
title: "CellValue.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellValue. يحصل أو يضبط نوع قيمة الخلية"
type: docs
url: /ar/net/aspose.cells/cellvalue/type/
---
## CellValue.Type property

يحصل أو يعيّن نوع قيمة الخلية.

```csharp
public CellValueType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين قيم خلايا مختلفة بأنواع مختلفة
            worksheet.Cells["A1"].PutValue("Text Value"); // Text type
            worksheet.Cells["A2"].PutValue(123.45);       // Numeric type
            worksheet.Cells["A3"].PutValue(true);        // Boolean type
            worksheet.Cells["A4"].PutValue("=1/0");       // Error type (will show #DIV/0!)

            // معالجة كل خلية وإظهار خاصية Type
            for (int i = 0; i < 4; i++)
            {
                Cell cell = worksheet.Cells[0, i];
                CellValue value = (CellValue)cell.Value;
                
                Console.WriteLine($"Cell {cell.Name} - Original Type: {value.Type}, Value: {value.Value}");

                // إظهار تغيير النوع للقيم الخطأ
                if (value.Type == CellValueType.IsError && "#DIV/0!".Equals(value.Value))
                {
                    value.Type = CellValueType.IsNull;
                    Console.WriteLine($"Changed error to null - New Type: {value.Type}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* enum [CellValueType](../../cellvaluetype/)
* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


