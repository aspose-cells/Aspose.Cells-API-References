---
title: "StyleFlag.All"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Toutes les propriétés seront appliquées"
type: docs
url: /fr/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

Toutes les propriétés seront appliquées.

```csharp
public bool All { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer un style avec un arrière-plan rouge uni
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // Créer un indicateur de style avec la propriété All définie sur true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // Appliquer le style à la première colonne
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // Vérifier que le style a été appliqué aux cellules de la colonne
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


