---
title: "CellValue.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellValue. تحصل أو تضبط قيمة الخلية"
type: docs
url: /ar/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

يحصل أو يعيّن قيمة الخلية.

```csharp
public object Value { get; set; }
```

### ملاحظات

يجب أن تكون القيمة من النوع الصحيح للكائن المتطابق مع [`Type`](../type/):

| **Type** | **Value** |
| --- | --- |
| IsNull | null، أي كائن آخر سيتم تجاهله |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | سلسلة خطأ مثل "#VALUE!", "#NAME?", ... |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            worksheet.Cells["A1"].PutValue(cellValue.Value);

            workbook.Save("CellValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


