---
title: "Cell.IsDynamicArrayFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si la formule de la cellule est une formule de tableau dynamique true ou une formule de tableau hérité false"
type: docs
url: /fr/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Indique si la formule de la cellule est une formule de tableau dynamique (true) ou une formule de tableau héritée (false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définissez une formule de tableau dynamique dans la cellule A1
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // Vérifiez si la cellule contient une formule de tableau dynamique
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // Enregistrez le classeur
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


