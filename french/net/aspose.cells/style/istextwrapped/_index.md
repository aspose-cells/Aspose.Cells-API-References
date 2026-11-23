---
title: "Style.IsTextWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne"
type: docs
url: /fr/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Obtient ou définit une valeur indiquant si le texte à l'intérieur d'une cellule est renvoyé à la ligne.

```csharp
public bool IsTextWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // Définir un texte long dans la cellule
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // Activer le renvoi à la ligne du texte
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // Ajuster la hauteur de la ligne pour afficher le texte renvoyé à la ligne
            ws.AutoFitRow(0);
            
            // Enregistrez le classeur
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


