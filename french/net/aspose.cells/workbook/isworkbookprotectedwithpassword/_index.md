---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Indique si la structure ou la fenêtre est protégée par un mot de passe"
type: docs
url: /fr/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Indique si la structure ou la fenêtre est protégée par mot de passe.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Créer une nouvelle instance de Workbook
            Workbook workbook = new Workbook();

            // Vérifier si le classeur est protégé par un mot de passe (devrait être faux pour un nouveau classeur)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Protéger le classeur avec un mot de passe
            workbook.Protect(ProtectionType.All, "password123");

            // Vérifier à nouveau (devrait être vrai)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Déprotéger le classeur
            workbook.Unprotect("password123");

            // Vérification finale (devrait être faux à nouveau)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Libérer le classeur
            workbook.Dispose();
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


