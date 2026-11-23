---
title: "StyleFlag.FontBold"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre de gras de police sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

Le paramètre de gras de police sera appliqué.

```csharp
public bool FontBold { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style gras
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Appliquer le style gras à la ligne 2 avec StyleFlag uniquement pour FontBold
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // Mettre une valeur dans la cellule pour démontrer le style
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


