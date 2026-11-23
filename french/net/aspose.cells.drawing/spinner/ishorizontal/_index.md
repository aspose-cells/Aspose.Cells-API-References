---
title: "Spinner.IsHorizontal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Spinner. Indique si c'est une barre de défilement horizontale"
type: docs
url: /fr/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

Indique si c'est une barre de défilement horizontale.

```csharp
public bool IsHorizontal { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Ajouter une forme de spinner à la feuille de calcul
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // Définir les propriétés du Spinner
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // Démontrer la propriété IsHorizontal (lecture et écriture)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // Basculer l'orientation
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // Enregistrez le classeur
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


