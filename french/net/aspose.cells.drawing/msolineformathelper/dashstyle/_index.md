---
title: "MsoLineFormatHelper.DashStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormatHelper. Obtient ou définit le style de tiret pour la ligne spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Obtient ou définit le style de tiret pour la ligne spécifiée.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // Affiche la valeur actuelle de DashStyle
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // Définir une nouvelle valeur DashStyle (puisqu'elle est en lecture/écriture)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // Enregistrer le résultat
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


