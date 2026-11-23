---
title: "Style.IndentLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Représente le niveau d'indentation pour la cellule ou la plage. Ne peut être qu'un entier de 0 à 250"
type: docs
url: /fr/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Représente le niveau d'indentation pour la cellule ou la plage. Ne peut être qu'un entier compris entre 0 et 250.

```csharp
public int IndentLevel { get; set; }
```

### Remarques

Si le type d'alignement horizontal du texte est défini sur une valeur autre que gauche ou droite, le niveau d'indentation sera réinitialisé à zéro.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez différents niveaux d'indentation pour les cellules
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // Enregistrez le classeur
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


