---
title: "Cell.IsFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si la cellule spécifiée contient une formule"
type: docs
url: /fr/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Indique si la cellule spécifiée contient une formule.

```csharp
public bool IsFormula { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une formule à la cellule A1
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // Ajouter une valeur simple à la cellule A2
            worksheet.Cells["A2"].PutValue("Test");
            
            // Vérifier si les cellules contiennent des formules
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


