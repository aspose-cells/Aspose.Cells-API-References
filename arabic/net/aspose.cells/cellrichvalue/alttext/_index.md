---
title: "CellRichValue.AltText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellRichValue. يحصل على النص البديل المرتبط بالصورة"
type: docs
url: /ar/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

يحصل على النص البديل المرتبط بالصورة.

```csharp
public virtual string AltText { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyAltTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["C4"];
            
            cell.GetRichValue().AltText = "test alt text";
            
            Console.WriteLine("AltText: " + cell.GetRichValue().AltText);
        }
    }
}
```

### انظر أيضًا

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


