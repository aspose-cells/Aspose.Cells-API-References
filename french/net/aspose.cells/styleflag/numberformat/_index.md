---
title: "StyleFlag.NumberFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre de format numérique sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Le paramètre de format numérique sera appliqué.

```csharp
public bool NumberFormat { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Définir la valeur de la cellule
            sheet.Cells[0, 0].Value = 1234.56;
            
            // Créer un style de format numérique personnalisé
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // Appliquer uniquement le format numérique en utilisant StyleFlag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // Appliquer le style à la plage de cellules (qualifier complètement le type Range)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // Enregistrer et vérifier
            workbook.Save("output_number_format.ods");
            
            // Recharger pour vérifier
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


