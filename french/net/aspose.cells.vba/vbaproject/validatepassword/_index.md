---
title: "VbaProject.ValidatePassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaProject. Valide le mot de passe de protection"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Valide le mot de passe de protection.

```csharp
public bool ValidatePassword(string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot de passe | String | le mot de passe |

### Valeur de retour

Indique si le mot de passe est le mot de passe de protection de ce projet VBA

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Créer un objet classeur à partir d'un fichier Excel d'exemple contenant un projet VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Valider le mot de passe du projet VBA
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // Afficher le résultat de la validation
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


