---
title: VbaProject.Name
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Gets and sets the name of the VBA project
type: docs
url: /net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

Gets and sets the name of the VBA project.

```csharp
public string Name { get; set; }
```

### Examples

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

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


