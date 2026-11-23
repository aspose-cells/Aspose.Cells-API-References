---
title: "Cell.SetCharacters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Définit le format texte enrichi de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

Définit le format de texte riche de la cellule.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| caractères | FontSetting[] | Tous les objets Characters. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellMethodSetCharactersWithFontSettingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Définir la valeur de la cellule pour appliquer le formatage de texte enrichi
            cell.Value = "Hello World!";

            try
            {
                // Créer des paramètres de police pour différentes parties du texte
                FontSetting[] fontSettings = new FontSetting[2];

                // Formater les 5 premiers caractères (Hello) en gras rouge
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // Formater les caractères restants ( World!) en italique bleu
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // Appliquer les paramètres de caractères formatés en utilisant SetCharacters
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


