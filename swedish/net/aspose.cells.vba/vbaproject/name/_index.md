---
title: "VbaProject.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject egenskap. Hämtar och anger namnet på VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

Hämtar och anger namnet på VBA-projektet.

```csharp
public string Name { get; set; }
```

### Exempel

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

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


