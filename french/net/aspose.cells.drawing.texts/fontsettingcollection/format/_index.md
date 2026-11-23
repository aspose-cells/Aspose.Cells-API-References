---
title: "FontSettingCollection.Format"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontSettingCollection. Formater le texte avec le paramètre de police"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

Formate le texte avec le paramètre de police.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index de départ. |
| longueur | Int32 | La longueur. |
| police | Police | La police. |
| flag | StyleFlag | Les indicateurs de la police. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
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
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // Créer un style et définir ses propriétés de police
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // Créer un drapeau de style pour spécifier quelles propriétés de police appliquer
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // Formater les caractères de l'index 7 à 11 (le mot "Text")
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // Enregistrer le classeur pour montrer l'effet
                workbook.Save("FontSettingCollectionFormatDemo.xlsx");
                Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


