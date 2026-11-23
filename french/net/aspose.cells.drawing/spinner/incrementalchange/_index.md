---
title: "Spinner.IncrementalChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Spinner. Obtient ou définit le montant d'incrémentation de la barre de défilement ou du spinner lors d'un défilement d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Obtient ou définit la quantité d'incrémentation d'une ligne de la barre de défilement ou du sélecteur.

```csharp
public int IncrementalChange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un contrôle spinner
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // Définir les propriétés du Spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // Vérifier et afficher la valeur IncrementalChange
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // Modifier et vérifier à nouveau
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // Enregistrez le classeur
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


