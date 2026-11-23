---
title: "Shape.FormatCharacters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Formate certains caractères avec le réglage de police"
type: docs
url: /fr/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Formate certains caractères avec le paramètre de police.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index de départ. |
| longueur | Int32 | La longueur. |
| police | Police | Le paramètre de police. |
| flag | StyleFlag | Le drapeau du paramètre de police. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une zone de texte à la feuille de calcul
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // Créer une police avec les propriétés souhaitées
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Créer un indicateur de style pour spécifier quelles propriétés appliquer
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // Appliquer le formatage à des caractères spécifiques
            textBox.FormatCharacters(0, 6, font, flag);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


