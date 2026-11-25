---
title: "CellsHelper.AltStartPath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di CellsHelper. Ottiene o imposta il percorso di avvio alternativo a cui si fa riferimento da alcune referenze di formule esterne"
type: docs
url: /it/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

Ottiene o imposta il percorso di avvio alternativo, a cui si fa riferimento da alcune formule esterne.

```csharp
public static string AltStartPath { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // Imposta il percorso di avvio alternativo
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // Imposta anche altre proprietà rilevanti per la dimostrazione
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // Visualizza i percorsi per dimostrare l'uso della proprietà
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // Esempio di come questi percorsi potrebbero essere usati
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


