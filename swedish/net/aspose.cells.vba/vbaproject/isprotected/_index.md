---
title: "VbaProject.IsProtected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject-egenskap. Anger om detta VBA-projekt är skyddat"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

Anger om detta VBA-projekt är skyddat.

```csharp
public bool IsProtected { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Läs in en exempel-Excel-fil med oskyddat VBA-projekt
            Workbook wb = new Workbook("load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Läs in en exempel-Excel-fil med skyddat VBA-projekt
            wb = new Workbook("load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Läs in en exempel-Excel-fil med skyddat och låst VBA-projekt
            wb = new Workbook("load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


