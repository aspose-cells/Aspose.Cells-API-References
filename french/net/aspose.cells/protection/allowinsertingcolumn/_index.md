---
title: "Protection.AllowInsertingColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Protection property. Représente si l'insertion de colonnes est autorisée sur une feuille de calcul protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

Représente si l'insertion de colonnes est autorisée sur une feuille de calcul protégée

```csharp
public bool AllowInsertingColumn { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir les paramètres de protection
            Protection protection = worksheet.Protection;

            // Définir AllowInsertingColumn sur true
            protection.AllowInsertingColumn = true;

            // Vérifiez le paramètre
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // Protéger la feuille de calcul avec un mot de passe (en utilisant la méthode Workbook.Protect)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

            // Enregistrez le classeur
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


