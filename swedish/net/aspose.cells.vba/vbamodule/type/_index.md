---
title: "VbaModule.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModule-egenskap. Hämtar modulens typ"
type: docs
url: /sv/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Hämtar modulens typ.

```csharp
public VbaModuleType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med exempel på makroaktiverad fil
            Workbook wb = new Workbook("example.xlsm");
            
            // Få åtkomst till VBA-projekt och moduler
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // Visa modultyper och namn
            for (int i = 0; i < modules.Count; i++)
            {
                Console.WriteLine($"Module Name: {modules[i].Name}");
                Console.WriteLine($"Module Type: {modules[i].Type}");
                Console.WriteLine();
            }
            
            wb.Save("output.xlsm");
        }
    }
}
```

### Se även

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


