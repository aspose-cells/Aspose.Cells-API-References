---
title: "CellsHelper.AltStartPath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsHelper. Obtient ou définit le chemin de démarrage alternatif qui est référencé par certaines références de formules externes"
type: docs
url: /fr/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

Obtient ou définit le chemin de démarrage alternatif, qui est référencé par certaines références de formules externes.

```csharp
public static string AltStartPath { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // Définir le chemin de démarrage alternatif
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // Définissez également d'autres propriétés pertinentes pour la démonstration
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // Affichez les chemins pour démontrer l'utilisation de la propriété
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // Exemple de la façon dont ces chemins peuvent être utilisés
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


