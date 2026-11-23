---
title: "VbaProject.IslockedForViewing"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Indique si ce projet VBA est verrouillé en vue"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/islockedforviewing/
---
## VbaProject.IslockedForViewing property

Indique si ce projet VBA est verrouillé en vue.

```csharp
[Obsolete("Use VbaProject.IsLockedForView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IslockedForViewing { get; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété VbaProject.IsLockedForView. Cette propriété sera supprimée 12 mois plus tard à compter de juillet 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

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
            // Créer un classeur d'exemple avec le projet VBA
            Workbook wb = new Workbook();
            // Créer une nouvelle feuille de calcul pour garantir que le projet VBA est créé
            wb.Worksheets.Add();
            
            // Démontrer la propriété IslockedForViewing
            Console.WriteLine("Initial state:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Protéger et verrouiller pour la visualisation
            wb.VbaProject.Protect(true, "password123");
            Console.WriteLine("After protecting and locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Protéger sans verrouiller pour la visualisation
            wb.VbaProject.Protect(false, "password456");
            Console.WriteLine("After protecting without locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Supprimer la protection
            wb.VbaProject.Protect(true, "");
            Console.WriteLine("After removing protection:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}");
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


