---
title: "FontSettingCollection.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSettingCollection."
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Définir du texte
            fontSettingCollection.Text = "Sample Text";

            try
            {
                // Créer un autre FontSettingCollection pour la comparaison
                var anotherTextBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var anotherFontSettingCollection = anotherTextBox.TextBody;
                anotherFontSettingCollection.Text = "Sample Text";

                // Appeler la méthode Equals pour comparer les deux collections
                bool areEqual = fontSettingCollection.Equals(anotherFontSettingCollection);

                // Afficher le résultat
                Console.WriteLine($"Are the FontSettingCollections equal? {areEqual}");

                // Enregistrez le classeur
                workbook.Save("FontSettingCollectionEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Equals: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


