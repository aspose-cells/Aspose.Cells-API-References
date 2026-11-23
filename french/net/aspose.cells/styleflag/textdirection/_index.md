---
title: "StyleFlag.TextDirection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le réglage de la direction du texte sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

Le paramètre de direction du texte sera appliqué.

```csharp
public bool TextDirection { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // Créer un style et définir la direction du texte
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // Créer un indicateur de style et activer l'indicateur TextDirection
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // Appliquer le style à la cellule avec l'indicateur de style
            cell.SetStyle(style, styleFlag);

            // Afficher la direction du texte actuelle
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Modifier la direction du texte et appliquer à nouveau
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Enregistrez le classeur
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


