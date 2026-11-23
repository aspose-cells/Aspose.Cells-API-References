---
title: "FontSettingCollection.InsertText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSettingCollection. Insère l'index à la position"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/inserttext/
---
## FontSettingCollection.InsertText method

Insère l'index à la position.

```csharp
public void InsertText(int index, string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index de départ. |
| texte | String | Le texte. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var fontSettingCollection = textBox.TextBody;

            // Définir le texte initial
            fontSettingCollection.Text = "Initial Text";

            try
            {
                // Appeler la méthode InsertText pour insérer du texte à l'index 7
                fontSettingCollection.InsertText(7, " Inserted");

                // Afficher le texte modifié
                Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
                
                // Enregistrez le classeur
                workbook.Save("FontSettingCollectionInsertTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertText method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


