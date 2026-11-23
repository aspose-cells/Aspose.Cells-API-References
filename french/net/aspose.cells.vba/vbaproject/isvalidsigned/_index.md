---
title: "VbaProject.IsValidSigned"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Indique si la signature du projet VBA est valide ou non"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

Indique si la signature du projet VBA est valide ou non.

```csharp
public bool IsValidSigned { get; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsValidSignedDemo
    {
        public static void Run()
        {
            // Charger un classeur d'exemple avec un projet VBA signé
            Workbook wb = new Workbook("example.xlsm");
            
            // Vérifier si le projet VBA est signé et si la signature est valide
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // Enregistrer et recharger pour vérifier que la signature persiste
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


