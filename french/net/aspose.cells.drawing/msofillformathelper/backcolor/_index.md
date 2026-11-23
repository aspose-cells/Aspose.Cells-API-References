---
title: "MsoFillFormatHelper.BackColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormatHelper. Obtient et définit la couleur de fond du fichier"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Obtient et définit la couleur d'arrière-plan du fichier.

```csharp
public Color BackColor { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une étiquette juste pour avoir du contenu dans la feuille
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper n’expose pas de constructeur public, utilisez la réflexion pour l’instancier
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Définir BackColor à une couleur connue (par ex., LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // Lire la valeur de BackColor et l’afficher
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // Optionnellement, vous pouvez également lire ForeColor pour montrer qu’il reste par défaut
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Enregistrez le classeur – le helper de remplissage n’est pas attaché à une forme,
                // mais l’enregistrement montre que le code s’est exécuté sans erreur.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


