---
title: "Cell.BoolValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la valeur booléenne contenue dans la cellule"
type: docs
url: /fr/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Obtient la valeur booléenne contenue dans la cellule.

```csharp
public bool BoolValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // Définir une formule qui s'évalue à une valeur booléenne
            cell.Formula = "=2.01>2";
            
            // Calculer la formule pour obtenir le résultat
            workbook.CalculateFormula();
            
            // Démontrer la propriété BoolValue
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


