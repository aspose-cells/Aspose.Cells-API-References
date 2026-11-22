---
title: "Range.IsBlank"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تشير إلى ما إذا كان النطاق يحتوي على قيم"
type: docs
url: /ar/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

يشير إلى ما إذا كان النطاق يحتوي على قيم.

```csharp
public bool IsBlank()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نطاق والتحقق مما إذا كان فارغًا (يجب أن يكون صحيحًا)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // ضع قيمة في خلية واحدة وتحقق مرة أخرى (يجب أن يكون خاطئًا)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


