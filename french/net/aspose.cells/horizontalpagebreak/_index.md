---
title: "Classe HorizontalPageBreak"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.HorizontalPageBreak. Encapsule l'objet qui représente un saut de page horizontal"
type: docs
url: /fr/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Encapsule l'objet qui représente un saut de page horizontal.

```csharp
public class HorizontalPageBreak
```

## Propriétés

| Nom | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Obtient l'indice de colonne de fin de ce saut de page horizontal. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Obtient l'indice de ligne basé à zéro. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Obtient l'indice de colonne de début de ce saut de page horizontal. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un saut de page à la cellule Y30
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Récupérez le saut de page horizontal nouvellement ajouté
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Affichez les propriétés du saut de page horizontal
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Enregistrez le classeur
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


