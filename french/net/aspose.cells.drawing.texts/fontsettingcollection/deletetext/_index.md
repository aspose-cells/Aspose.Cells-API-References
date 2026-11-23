---
title: "FontSettingCollection.DeleteText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSettingCollection. Supprimer certains caractères"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

Supprime certains caractères.

```csharp
public void DeleteText(int index, int count)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index de départ. |
| nombre | Int32 | Le nombre de caractères. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Définir le texte initial
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // Afficher le texte original
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // Appelez la méthode DeleteText pour supprimer 7 caractères à partir de l'index 5
                fontSettingCollection.DeleteText(5, 7);

                // Afficher le texte modifié
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // Enregistrez le classeur
                workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


