---
title: "Cells.PreserveString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées en tant que chaînes. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

Obtient ou définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées sous forme de chaînes. La valeur par défaut est false.

```csharp
public bool PreserveString { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la propriété PreserveString sur true
            cells.PreserveString = true;

            // Ajouter des valeurs de chaîne aux cellules
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // Accéder aux valeurs (elles seront conservées en tant que chaînes)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // Enregistrez le classeur
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // Charger le classeur enregistré pour vérifier la conservation
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // Afficher les valeurs conservées
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // Démontrer la comparaison de la propriété PreserveString
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


