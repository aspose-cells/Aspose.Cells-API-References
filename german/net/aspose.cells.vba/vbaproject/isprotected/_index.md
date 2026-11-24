---
title: "VbaProject.IsProtected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Eigenschaft. Gibt an, ob dieses VBA-Projekt geschützt ist"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

Gibt an, ob dieses VBA-Projekt geschützt ist.

```csharp
public bool IsProtected { get; }
```

### Beispiele

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
            // Laden Sie eine Beispiel-Excel-Datei mit ungeschütztem VBA-Projekt
            Workbook wb = new Workbook("load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Laden Sie eine Beispiel-Excel-Datei mit geschütztem VBA-Projekt
            wb = new Workbook("load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Laden Sie eine Beispiel-Excel-Datei mit geschütztem und gesperrtem VBA-Projekt
            wb = new Workbook("load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
        }
    }
}
```

### Siehe auch

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


