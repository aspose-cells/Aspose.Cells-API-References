---
title: "MsoLineFormatHelper.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormatHelper. Indique si l'objet est visible"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Indique si l'objet est visible.

```csharp
public bool IsVisible { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
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

                // Affiche la valeur actuelle de IsVisible
                Console.WriteLine("Current IsVisible: " + lineFormat.IsVisible);

                // Définir une nouvelle valeur IsVisible (puisqu'elle est en lecture/écriture)
                lineFormat.IsVisible = false;
                Console.WriteLine("Updated IsVisible: " + lineFormat.IsVisible);

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("Line visibility has been updated to: " + lineFormat.IsVisible);

                // Enregistrer le résultat
                workbook.Save("IsVisibleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line visibility.");
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


