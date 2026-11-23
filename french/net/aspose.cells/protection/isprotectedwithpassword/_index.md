---
title: "Protection.IsProtectedWithPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Protection property. Indique si la feuille de calcul est protégée par mot de passe"
type: docs
url: /fr/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

Indique si la feuille de calcul est protégée par un mot de passe.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder aux paramètres de protection de la feuille de calcul
            Protection protection = worksheet.Protection;

            // Définir le mot de passe de protection
            protection.Password = "test123";

            // Vérifier si la feuille de calcul est protégée par mot de passe
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // Enregistrez le classeur
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


