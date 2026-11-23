---
title: "StyleFlag.FontStrike"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le réglage de la police barrée sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

Le paramètre de barré de police sera appliqué.

```csharp
public bool FontStrike { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Créer un objet style et définir FontStrike à true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Créer un indicateur de style et activer l'indicateur FontStrike
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Appliquer le style à la cellule avec l'indicateur de style
            cell.SetStyle(style, styleFlag);

            // Afficher l'état actuel de FontStrike
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // Créer une autre cellule pour démontrer du texte non barré
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // Enregistrer le classeur pour voir les effets
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


