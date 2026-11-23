---
title: "Worksheet.Cells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient la collection Cells"
type: docs
url: /fr/net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Obtient la collection [`Cells`](../../cells/).

```csharp
public Cells Cells { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de cellules
            Cells cells = worksheet.Cells;
            
            // Définir les valeurs dans les cellules
            cells["A1"].PutValue("Item");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);
            
            // Définir la formule pour calculer le total
            cells["A4"].PutValue("Total:");
            cells["B4"].Formula = "=SUM(B2:B3)";
            
            // Calculer les formules
            workbook.CalculateFormula();
            
            // Afficher les valeurs des cellules
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);
            Console.WriteLine("B2: " + cells["B2"].StringValue);
            Console.WriteLine("A3: " + cells["A3"].StringValue);
            Console.WriteLine("B3: " + cells["B3"].StringValue);
            Console.WriteLine("A4: " + cells["A4"].StringValue);
            Console.WriteLine("B4: " + cells["B4"].StringValue + " (Formula: " + cells["B4"].Formula + ")");
            
            // Enregistrer le classeur
            workbook.Save("CellsPropertyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


