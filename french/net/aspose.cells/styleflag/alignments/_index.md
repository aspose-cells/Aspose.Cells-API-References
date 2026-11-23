---
title: "StyleFlag.Alignments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre d'alignement sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

Le réglage d'alignement sera appliqué.

```csharp
public bool Alignments { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Créez un objet style et définissez les propriétés d'alignement
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // Créer un indicateur de style et activer les propriétés d'alignement
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // Appliquer le style à la cellule avec l'indicateur de style
            cell.SetStyle(style, styleFlag);

            // Afficher les paramètres d'alignement actuels
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Modifier l'indicateur de style pour désactiver les propriétés d'alignement
            styleFlag.Alignments = false;
            
            // Créer un nouveau style avec un alignement différent
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // Appliquer le nouveau style - les alignements ne changeront pas car l'indicateur est false
            cell.SetStyle(newStyle, styleFlag);

            // Afficher les paramètres d'alignement inchangés
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Enregistrez le classeur
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


