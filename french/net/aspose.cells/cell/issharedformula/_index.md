---
title: "Cell.IsSharedFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si la formule de la cellule fait partie d'une formule partagée"
type: docs
url: /fr/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Indique si la formule de la cellule fait partie d'une formule partagée.

```csharp
public bool IsSharedFormula { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir une formule partagée dans une plage
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // Vérifier si les cellules contiennent une formule partagée
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


