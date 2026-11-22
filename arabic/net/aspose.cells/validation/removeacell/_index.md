---
title: "Validation.RemoveACell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة التحقق. إزالة إعدادات التحقق في الخلية"
type: docs
url: /ar/net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

إزالة إعدادات التحقق في الخلية.

```csharp
public void RemoveACell(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة التحقق من البيانات إلى الخلية الأولى
            Validation validation = worksheet.Validations[0];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.Type = ValidationType.List;
            validation.Formula1 = "1,2,3";
            
            // إضافة خلية أخرى إلى التحقق
            validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
            
            // إزالة الخلية الثانية من التحقق
            validation.RemoveACell(1, 1);
            
            Console.WriteLine("Cell removed from validation successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


