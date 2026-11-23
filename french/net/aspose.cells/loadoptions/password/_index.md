---
title: "LoadOptions.Password"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LoadOptions property. Obtient et définit le mot de passe du classeur"
type: docs
url: /fr/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Obtient et définit le mot de passe du classeur.

```csharp
public string Password { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Créer des options de chargement et définir le mot de passe
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // Charger le classeur protégé par mot de passe
            Workbook workbook = new Workbook("protected.xlsx", options);

            // Supprimer la protection par mot de passe après le chargement
            workbook.Settings.Password = null;

            // Enregistrez le classeur non protégé
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


