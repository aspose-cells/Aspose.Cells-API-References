---
title: "FontSettingCollection.Replace"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSettingCollection. Remplace le texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Remplace le texte.

```csharp
public void Replace(int index, int count, string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index de départ. |
| nombre | Int32 | Le nombre de caractères. |
| texte | String | Le texte. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // Appelez la méthode Replace pour remplacer 8 caractères à partir de l'index 9 par du nouveau texte
                fontSettingCollection.Replace(9, 8, "replaced");

                // Afficher le texte modifié
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // Enregistrez le classeur
                workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Remplace le texte.

```csharp
public void Replace(string oldValue, string newValue)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| oldValue | String | L'ancien texte. |
| newValue | String | Le nouveau texte. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme et définir le texte
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // Remplacer le texte dans la forme
            shape.TextBody.Replace("３４", "ABC");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


