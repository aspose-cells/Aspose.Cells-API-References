---
title: "Protection.AllowDeletingRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Indique si la suppression de lignes est autorisée sur une feuille de calcul protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Représente si la suppression de lignes est autorisée sur une feuille de calcul protégée.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Remarques

Les lignes contenant les cellules à supprimer doivent être déverrouillées lorsque la feuille est protégée, et l'option "Select unlocked cells" doit être activée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir les paramètres de protection
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // Protéger la feuille de calcul
            sheet.Protect(ProtectionType.All);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Charger le classeur enregistré pour vérifier les paramètres
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // Vérifier AllowDeletingRow et les autres propriétés
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


