---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Représente si l'utilisateur est autorisé à sélectionner les cellules déverrouillées sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Représente si l'utilisateur est autorisé à sélectionner les cellules déverrouillées sur une feuille de calcul protégée.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Protéger la feuille avec toutes les options de protection
            Protection protection = worksheet.Protection;
            
            // Définir AllowSelectingUnlockedCell sur true
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // Appliquer la protection avec un mot de passe
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Vérifiez le paramètre
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

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


