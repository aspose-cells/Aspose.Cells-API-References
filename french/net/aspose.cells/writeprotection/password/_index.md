---
title: "WriteProtection.Password"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WriteProtection. Définit le mot de passe protégé pour modifier le fichier"
type: docs
url: /fr/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Définit le mot de passe de protection pour modifier le fichier.

```csharp
public string Password { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le mot de passe de protection en écriture
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Enregistrez le classeur
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### Voir aussi

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


