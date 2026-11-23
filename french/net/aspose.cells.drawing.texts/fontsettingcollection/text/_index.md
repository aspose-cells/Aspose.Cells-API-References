---
title: "FontSettingCollection.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontSettingCollection. Obtient et définit le texte de la forme"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/text/
---
## FontSettingCollection.Text property

Obtient et définit le texte de la forme.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            try
            {
                // Définir le texte initial
                fontSettingCollection.Text = "Initial Text Value";
                Console.WriteLine("Initial Text value: " + fontSettingCollection.Text);

                // Modifiez le texte
                fontSettingCollection.Text = "Modified Text Value";
                Console.WriteLine("Modified Text value: " + fontSettingCollection.Text);

                // Démontrer l'ajout de texte
                fontSettingCollection.AppendText(" (Appended)");
                Console.WriteLine("After AppendText: " + fontSettingCollection.Text);

                // Enregistrez le classeur
                workbook.Save("FontSettingCollectionTextDemo.xlsx");
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

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


