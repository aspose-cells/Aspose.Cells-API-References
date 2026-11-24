---
title: "VbaModule.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModule-Eigenschaft. Gibt den Typ des Moduls zurück"
type: docs
url: /de/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Ermittelt den Typ des Moduls.

```csharp
public VbaModuleType Type { get; }
```

### Beispiele

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
            // Arbeitsmappe mit Beispiel-Makrodatei erstellen
            Workbook wb = new Workbook("example.xlsm");
            
            // Auf VBA-Projekt und -Module zugreifen
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // Modultypen und -namen anzeigen
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

### Siehe auch

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


