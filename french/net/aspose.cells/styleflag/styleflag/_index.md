---
title: "StyleFlag.StyleFlag"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur StyleFlag. Crée un objet avec tous les indicateurs à false"
type: docs
url: /fr/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Construit un objet avec tous les indicateurs à false.

```csharp
public StyleFlag()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style gras
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Appliquer le style à la ligne 9 avec le constructeur StyleFlag
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // Mettre une valeur dans la cellule et vérifier le style
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


