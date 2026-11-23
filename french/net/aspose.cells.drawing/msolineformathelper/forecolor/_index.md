---
title: "MsoLineFormatHelper.ForeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormatHelper. Obtient et définit la couleur de premier plan de la ligne de bordure"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Obtient et définit la couleur de premier plan de la ligne de bordure.

```csharp
public Color ForeColor { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyForeColorDemo
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

                // Afficher la valeur actuelle de ForeColor
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // Définir un nouveau ForeColor (car il est en lecture/écriture)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // Enregistrer le résultat
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
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


