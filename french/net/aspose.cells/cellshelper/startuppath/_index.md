---
title: "CellsHelper.StartupPath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsHelper. Obtient ou définit le chemin de démarrage auquel font référence certaines références de formule externes"
type: docs
url: /fr/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Obtient ou définit le chemin de démarrage, qui est référencé par certaines références de formules externes.

```csharp
public static string StartupPath { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // Définir le chemin de démarrage
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // Afficher le chemin de démarrage
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // Démontrer des propriétés supplémentaires de CellsHelper
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


