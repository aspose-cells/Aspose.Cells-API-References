---
title: "MsoLineFormatHelper.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormatHelper. Retourne ou définit le degré de transparence du remplissage spécifié comme une valeur de 0,0 opaque à 1,0 clair"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformathelper/transparency/
---
## MsoLineFormatHelper.Transparency property

Renvoie ou définit le degré de transparence du remplissage spécifié sous forme d'une valeur comprise entre 0.0 (opaque) et 1.0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyTransparencyDemo
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

                // Afficher la valeur actuelle de Transparency
                Console.WriteLine("Current Transparency: " + lineFormat.Transparency);

                // Définir une nouvelle valeur de Transparency (car il est en lecture/écriture)
                lineFormat.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + lineFormat.Transparency);

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("Line transparency has been updated to: " + lineFormat.Transparency);

                // Enregistrer le résultat
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line transparency.");
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


