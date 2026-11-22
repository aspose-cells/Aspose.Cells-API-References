---
title: "VbaProject.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. يحصل على اسم مشروع VBA ويضبطه"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

يحصل على اسم مشروع VBA ويضبطه.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Console.WriteLine("VBA Project Name: " + workbook.VbaProject.Name);
            workbook.Save("example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


