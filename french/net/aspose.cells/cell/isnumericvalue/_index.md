---
title: "Cell.IsNumericValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si la valeur de cette cellule est numérique, entier, double ou datetime"
type: docs
url: /fr/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Indique si la valeur de cette cellule est numérique (int, double et datetime).

```csharp
public bool IsNumericValue { get; }
```

### Remarques

S'applique également aux cellules de formule pour vérifier le résultat calculé

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter différents types de données aux cellules
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // Vérifier si les cellules contiennent des valeurs numériques
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // Démontrer l'utilisation avec une logique conditionnelle
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


