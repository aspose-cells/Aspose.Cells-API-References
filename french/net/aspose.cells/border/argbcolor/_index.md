---
title: "Border.ArgbColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Border. Obtient et définit la couleur avec une valeur ARGB 32 bits"
type: docs
url: /fr/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

Obtient et définit la couleur avec une valeur ARGB 32 bits.

```csharp
public int ArgbColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule B2 et définir une valeur
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // Obtenir le style et les bordures
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // Définir les propriétés de bordure incluant la couleur ARGB
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // Appliquer le style modifié à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("BorderArgbColorDemo.xlsx");

            // Vérifier que la couleur ARGB a été définie correctement
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### Voir aussi

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


