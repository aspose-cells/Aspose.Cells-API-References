---
title: "Cell.IsArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si la formule de la cellule est une formule de tableau"
type: docs
url: /fr/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Indique si la formule de la cellule est une formule matricielle.

```csharp
public bool IsArrayFormula { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une formule matricielle dans la cellule B2
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // Vérifier si la cellule contient une formule matricielle
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // Afficher le résultat
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // Enregistrez le classeur
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


