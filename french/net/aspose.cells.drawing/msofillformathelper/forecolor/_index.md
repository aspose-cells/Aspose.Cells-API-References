---
title: "MsoFillFormatHelper.ForeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormatHelper. Obtient et définit la couleur de premier plan du remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Obtient et définit la couleur de premier plan du remplissage.

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
    using System.Reflection;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une étiquette pour rendre l'exemple significatif
            worksheet.Cells["A1"].Value = "ForeColor Property Demo";

            try
            {
                // Créer une instance de MsoFillFormatHelper en utilisant la réflexion (pas de constructeur public)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Afficher la valeur par défaut de ForeColor
                Console.WriteLine($"Default ForeColor: {fillHelper.ForeColor}");

                // Définir une nouvelle valeur de ForeColor
                fillHelper.ForeColor = Color.FromArgb(255, 128, 0, 128); // Purple color
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");

                // Démontrer la récupération de la valeur de ForeColor
                Color currentColor = fillHelper.ForeColor;
                Console.WriteLine($"Current ForeColor (RGB): R={currentColor.R}, G={currentColor.G}, B={currentColor.B}");

                // Enregistrez le classeur pour démontrer une exécution réussie
                workbook.Save("ForeColorDemo.xlsx");

                Console.WriteLine("ForeColor property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColor demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


