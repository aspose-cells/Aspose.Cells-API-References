---
title: "VbaProject.IsSigned"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Indique si le code VBA est signé ou non"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

Indique si le code VBA est signé ou non.

```csharp
public bool IsSigned { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // Charger un fichier Excel d'exemple avec le projet VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Vérifier si le projet VBA est signé
            if (workbook.VbaProject.IsSigned)
            {
                Console.WriteLine("VBA project is signed.");
                Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
            }
            else
            {
                Console.WriteLine("VBA project is not signed.");
            }
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


