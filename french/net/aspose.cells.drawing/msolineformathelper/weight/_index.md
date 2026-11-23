---
title: "MsoLineFormatHelper.Weight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormatHelper. Retourne ou définit le poids de la ligne en unités de pt"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Renvoie ou définit l'épaisseur de la ligne, en unités de pt.

```csharp
public double Weight { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyWeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Créer une forme pour démontrer le formatage de ligne
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Obtenir le format de ligne
                MsoLineFormat lineFormat = shape.LineFormat;

                // Affiche la valeur actuelle de Weight
                Console.WriteLine("Current Line Weight: " + lineFormat.Weight);

                // Définir une nouvelle valeur Weight (puisqu'elle est en lecture/écriture)
                lineFormat.Weight = 2.5;
                Console.WriteLine("Updated Line Weight: " + lineFormat.Weight);

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("Line weight has been updated to: " + lineFormat.Weight);

                // Enregistrer le résultat
                workbook.Save("WeightDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line weight.");
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

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


