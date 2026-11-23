---
title: "Shape.GetCharacters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Retourne tous les objets Characters qui représentent une plage de caractères dans le texte"
type: docs
url: /fr/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

Retourne tous les objets Characters qui représentent une plage de caractères dans le texte .

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### Valeur de retour

Tous les objets Characters

### Remarques

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Shape.GetRichFormattings(). Cette méthode sera supprimée 12 mois plus tard, depuis novembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte à la feuille de calcul avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // Obtenir les caractères de la forme
            ArrayList characters = shape.GetCharacters();

            // Afficher les informations sur chaque caractère
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


