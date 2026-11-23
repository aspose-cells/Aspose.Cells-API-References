---
title: "WriteProtection.IsWriteProtected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WriteProtection. Indique si ce classeur est protégé en écriture"
type: docs
url: /fr/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Indique si ce classeur est protégé en écriture.

```csharp
public bool IsWriteProtected { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Activer la protection en écriture avec un mot de passe
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Vérifier si le classeur est protégé en écriture
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // Valider le mot de passe
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // Enregistrez le classeur
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // Charger le classeur enregistré pour vérifier la protection
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // Vérifier à nouveau l'état de la protection
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Voir aussi

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


