---
title: "FontSetting.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontSetting. Obtient le type de nœud de texte"
type: docs
url: /fr/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

Obtient le type de nœud de texte.

```csharp
public virtual TextNodeType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter du texte à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Obtenir les paramètres de police pour les caractères de la cellule
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // Afficher la valeur actuelle de Type
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // Démontrer comment le Type affecte le traitement du texte
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // Appliquer une mise en forme différente en fonction du Type
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // Enregistrer le résultat
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


