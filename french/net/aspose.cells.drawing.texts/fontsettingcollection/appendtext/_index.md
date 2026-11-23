---
title: "FontSettingCollection.AppendText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSettingCollection. Ajoute le texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

Ajoute le texte.

```csharp
public void AppendText(string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodAppendTextWithStringDemo
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
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // Appeler la méthode AppendText pour ajouter du texte supplémentaire
                fontSettingCollection.AppendText("World!");

                // Afficher le texte modifié
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // Enregistrez le classeur
                workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AppendText method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


