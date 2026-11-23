---
title: "TextOptions.Kerning"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextOptions. Spécifie la taille de police minimale à laquelle le crénage des caractères se produit pour ce run de texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

Spécifie la taille minimale de police à laquelle le crénage des caractères se produira pour cette séquence de texte.

```csharp
public double Kerning { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme avec du texte pour démontrer le crénage
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // Obtenez les TextOptions de la forme
            TextOptions textOptions = shape.TextOptions;

            // Affichez la valeur actuelle du crénage
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // Définir le crénage à 12 points (taille de police minimale pour que le crénage s'applique)
            textOptions.Kerning = 12;

            // Définissez une taille de police plus grande pour observer l'effet du crénage
            textOptions.Size = 24;

            // Enregistrer le classeur pour voir l'effet
            workbook.Save("PropertyKerningDemo.xlsx");

            // Créez une autre forme avec un crénage différent pour la comparaison
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // Enregistrez à nouveau avec les deux exemples
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


