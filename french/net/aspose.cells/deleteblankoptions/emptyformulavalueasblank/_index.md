---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteBlankOptions. Indique si une cellule sera considérée comme vide lorsqu'il s'agit d'une formule et que le résultat calculé est nul ou une chaîne vide. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Indique si une cellule sera considérée comme vide lorsqu'elle est une formule et que le résultat calculé est nul ou une chaîne vide. La valeur par défaut est false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Remarques

En général, l'utilisateur doit s'assurer que les formules ont été calculées avant l'opération de suppression lorsque cette propriété est vraie. Sinon, toutes les formules nouvellement créées par les API normales telles que [`Formula`](../../cell/formula/) seront considérées comme vides et pourraient être supprimées car avant le calcul leurs résultats calculés sont tous nuls.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplissez des données d'exemple
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Supprimer les lignes vides sans tenir compte des cellules vides de formule
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Réinitialiser les données
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Supprimer les lignes vides en traitant les cellules vides de formule comme vides
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### Voir aussi

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


