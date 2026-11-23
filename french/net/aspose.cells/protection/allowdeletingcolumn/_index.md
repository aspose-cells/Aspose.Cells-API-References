---
title: "Protection.AllowDeletingColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Représente si la suppression de colonnes est autorisée sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Représente si la suppression de colonnes est autorisée sur une feuille de calcul protégée.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Remarques

Les colonnes contenant les cellules à supprimer doivent être déverrouillées lorsque la feuille est protégée, et "Sélectionner les cellules déverrouillées" doit être activée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Activer la protection de la feuille
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // Vérifiez le paramètre
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // Essayez de supprimer une colonne (cela devrait fonctionner puisque AllowDeletingColumn est vrai)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // Désactiver la suppression de colonnes
            protection.AllowDeletingColumn = false;

            // Essayez de supprimer une autre colonne (cela devrait échouer)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


