---
title: "VbaModule.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaModule. Ottiene il tipo del modulo"
type: docs
url: /it/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Ottiene il tipo del modulo.

```csharp
public VbaModuleType Type { get; }
```

### Esempi

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
            // Crea una cartella di lavoro con un file di esempio abilitato alle macro
            Workbook wb = new Workbook("example.xlsm");
            
            // Accedi al progetto VBA e ai moduli
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // Visualizza i tipi e i nomi dei moduli
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

### Vedi anche

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


