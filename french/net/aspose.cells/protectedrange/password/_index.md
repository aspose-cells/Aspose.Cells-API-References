---
title: "ProtectedRange.Password"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ProtectedRange property. Représente le mot de passe pour protéger la plage"
type: docs
url: /fr/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Représente le mot de passe pour protéger la plage.

```csharp
public string Password { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de plages protégées
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Ajouter une plage protégée
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // Définir le mot de passe pour la plage protégée
            protectedRange.Password = "12345";

            // Enregistrez le classeur
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### Voir aussi

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


