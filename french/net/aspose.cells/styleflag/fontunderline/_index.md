---
title: "StyleFlag.FontUnderline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre de soulignement de police sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

Le paramètre de soulignement de police sera appliqué.

```csharp
public bool FontUnderline { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // Créer un objet de style et définir le soulignement de police
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // Créer un indicateur de style et activer l'indicateur de soulignement de police
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // Appliquer le style à la cellule avec l'indicateur de style
            cell.SetStyle(style, styleFlag);

            // Afficher l'état actuel du soulignement
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Modifier le type de soulignement en double
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Enregistrez le classeur
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


