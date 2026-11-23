---
title: "PasteOptions.OnlyVisibleCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PasteOptions. True signifie copier uniquement les cellules visibles"
type: docs
url: /fr/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

Vrai signifie ne copier que les cellules visibles.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // Créer un classeur avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Obtenir les cellules de la première feuille et remplir les données
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // Masquer certaines lignes et colonnes
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // Créer la plage source à copier
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // Obtenir les cellules de la deuxième feuille pour la destination
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // Créer des options de collage et définir OnlyVisibleCells
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // Copier uniquement les cellules visibles
            destRange.Copy(sourceRange, pasteOptions);
            
            // Afficher les résultats pour démontrer la fonctionnalité
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### Voir aussi

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


