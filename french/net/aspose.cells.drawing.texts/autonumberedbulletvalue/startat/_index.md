---
title: "AutoNumberedBulletValue.StartAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoNumberedBulletValue. Obtient et définit le numéro de départ de la puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/autonumberedbulletvalue/startat/
---
## AutoNumberedBulletValue.StartAt property

Obtient et définit le numéro de départ de la puce.

```csharp
public int StartAt { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyStartAtDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Créez une instance AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
                    StartAt = 3 // Setting the StartAt property
                };

                // Affichez la valeur actuelle de StartAt
                Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");

                // Modifiez la valeur de StartAt
                bullet.StartAt = 5;
                Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");

                // Créez une forme pour démontrer la puce dans le contexte
                var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "1. First Item\n2. Second Item";

                // Appliquez le style de puce (note : la méthode d'application réelle n’est pas affichée dans la réflexion)
                // À titre de démonstration, nous enregistrerons simplement le classeur
                workbook.Save("StartAtPropertyDemo.xlsx");
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

* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


