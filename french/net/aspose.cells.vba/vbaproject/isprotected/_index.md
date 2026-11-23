---
title: "VbaProject.IsProtected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Indique si ce projet VBA est protégé"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

Indique si ce projet VBA est protégé.

```csharp
public bool IsProtected { get; }
```

### Exemples

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
            // Charger un fichier Excel d'exemple avec un projet VBA non protégé
            Workbook wb = new Workbook("load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Charger un fichier Excel d'exemple avec un projet VBA protégé
            wb = new Workbook("load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Charger un fichier Excel d'exemple avec un projet VBA protégé et verrouillé
            wb = new Workbook("load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


