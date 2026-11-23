---
title: "Classe VerticalPageBreak"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.VerticalPageBreak. Encapsule l'objet qui représente un saut de page vertical"
type: docs
url: /fr/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Encapsule l'objet qui représente un saut de page vertical.

```csharp
public class VerticalPageBreak
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Obtient l'index de colonne du saut de page vertical. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Obtient l'index de ligne de fin du saut de page vertical. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Obtient l'index de ligne de début du saut de page vertical. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un saut de page vertical à la colonne G (index 6)
            worksheet.VerticalPageBreaks.Add("G5");

            // Enregistrez le classeur
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Accéder au saut de page vertical ajouté
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Afficher les propriétés du saut de page vertical
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


