---
title: "StyleFlag.FontScript"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "StyleFlag propriété. Le paramètre de script de police sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

Le paramètre de script de police sera appliqué.

```csharp
public bool FontScript { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Créer un objet de style et définir le script de police en indice
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // Créer un indicateur de style et activer l'indicateur FontScript
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // Appliquer le style à la cellule avec l'indicateur de style
            cell.SetStyle(style, styleFlag);

            // Afficher l'état actuel du script de police
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Modifier le script de police en exposant
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // Afficher l'état mis à jour du script de police
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Enregistrez le classeur
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


