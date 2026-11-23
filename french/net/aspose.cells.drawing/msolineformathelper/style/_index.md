---
title: "MsoLineFormatHelper.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormatHelper. Retourne un objet Style qui représente le style de la plage spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Renvoie un objet Style qui représente le style de la plage spécifiée.

```csharp
public MsoLineStyle Style { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
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

                // Obtenez le format de ligne directement (MsoLineFormatHelper semble être une classe d'assistance)
                // Comme nous ne pouvons pas instancier MsoLineFormatHelper directement, nous travaillerons avec la propriété LineFormat
                MsoLineFormat lineFormat = shape.LineFormat;

                // Affiche la valeur actuelle de Style
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // Définir un nouveau style (puisque Style est en lecture/écriture)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // Enregistrer le résultat
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


