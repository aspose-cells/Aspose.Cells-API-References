---
title: "Classe ConditionalFormattingIcon"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ConditionalFormattingIcon class. Représente l'icône personnalisée d'une règle de mise en forme conditionnelle"
type: docs
url: /fr/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

Représente l'icône personnalisée de la règle de mise en forme conditionnelle.

```csharp
public class ConditionalFormattingIcon
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | Obtient les données du jeu d'icônes. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | Obtient et définit l'index de l'icône dans le jeu d'icônes. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | Obtient et définit le type du jeu d'icônes. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Obtient les données d'image avec le paramètre de la cellule. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | Obtenir les données du jeu d'icônes |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la collection des mises en forme conditionnelles
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Ajouter un nouveau format conditionnel à la collection
            int index = cformattings.Add();
            
            // Accéder à la collection de conditions de formatage
            FormatConditionCollection fcs = cformattings[index];
            
            // Définir la zone de cellules où appliquer le format conditionnel
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Ajouter la zone de cellules à la collection de conditions de formatage
            fcs.AddArea(ca);
            
            // Ajouter une condition pour utiliser des jeux d'icônes
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Définir le type de jeu d'icônes
            fc.IconSet.Type = IconSetType.Arrows3;

            // Personnaliser les icônes individuelles du jeu d'icônes
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Enregistrez le classeur
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


