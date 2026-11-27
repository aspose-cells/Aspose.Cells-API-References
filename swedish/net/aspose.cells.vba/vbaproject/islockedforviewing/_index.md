---
title: "VbaProject.IslockedForViewing"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject-egenskap. Anger om detta VBA-projekt är låst för visning"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/islockedforviewing/
---
## VbaProject.IslockedForViewing property

Anger om detta VBA-projekt är låst för visning.

```csharp
[Obsolete("Use VbaProject.IsLockedForView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IslockedForViewing { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället VbaProject.IsLockedForView-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIslockedForViewingDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med VBA-projekt
            Workbook wb = new Workbook();
            // Skapa ett nytt kalkylblad för att säkerställa att VBA-projektet skapas
            wb.Worksheets.Add();
            
            // Demonstrera IslockedForViewing-egenskapen
            Console.WriteLine("Initial state:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Skydda och lås för visning
            wb.VbaProject.Protect(true, "password123");
            Console.WriteLine("After protecting and locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Skydda utan att låsa för visning
            wb.VbaProject.Protect(false, "password456");
            Console.WriteLine("After protecting without locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Ta bort skyddet
            wb.VbaProject.Protect(true, "");
            Console.WriteLine("After removing protection:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}");
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


