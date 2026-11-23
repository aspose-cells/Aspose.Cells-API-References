---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoNumberedBulletValue. Représente le schéma du numéro automatique"
type: docs
url: /fr/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

Représente le schéma du numéro automatique.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle instance AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // Afficher la valeur initiale d'AutonumberScheme
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // Définir une nouvelle valeur AutonumberScheme
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // Créer un classeur pour démontrer la puce dans le contexte
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Créer une forme avec du texte qui utilisera le style de puce
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // Remarque : L'application réelle du style de puce au texte nécessiterait des appels d'API supplémentaires
                // non affiché dans la réflexion. Nous enregistrerons simplement le classeur à titre de démonstration.
                workbook.Save("AutonumberSchemeDemo.xlsx");
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

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


