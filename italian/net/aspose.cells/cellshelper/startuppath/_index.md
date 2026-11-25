---
title: "CellsHelper.StartupPath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsHelper. Ottiene o imposta il percorso di avvio a cui si fa riferimento da alcuni riferimenti di formula esterni"
type: docs
url: /it/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Ottiene o imposta il percorso di avvio a cui si fa riferimento da alcune formule esterne.

```csharp
public static string StartupPath { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // Imposta il percorso di avvio
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // Visualizza il percorso di avvio
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // Dimostra le proprietà aggiuntive di CellsHelper
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


