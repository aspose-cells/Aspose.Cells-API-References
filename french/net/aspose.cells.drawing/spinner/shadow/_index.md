---
title: "Spinner.Shadow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Spinner. Indique si la forme possède un ombrage 3D"
type: docs
url: /fr/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

Indique si la forme possède un ombrage 3-D.

```csharp
public bool Shadow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un spinner à la feuille de calcul
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // Définir les propriétés du Spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // Démontrer la propriété Shadow
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // Enregistrez le classeur
            workbook.Save("SpinnerShadowDemo.xlsx");

            // Charger le classeur enregistré pour vérifier la propriété d'ombrage
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### Voir aussi

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


