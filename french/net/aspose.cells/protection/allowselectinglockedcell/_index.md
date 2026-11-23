---
title: "Protection.AllowSelectingLockedCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Indique si l’utilisateur est autorisé à sélectionner les cellules verrouillées sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

Représente si l'utilisateur est autorisé à sélectionner les cellules verrouillées sur une feuille de calcul protégée.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les paramètres de protection
            Protection protection = worksheet.Protection;
            
            // Démontrer la propriété AllowSelectingLockedCell
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // Modifier la propriété et afficher le changement
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // Protéger la feuille avec un mot de passe
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

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


