---
title: "PageSetup.Order"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente l'ordre que Microsoft Excel utilise pour numéroter les pages lors de l'impression d'une grande feuille de calcul"
type: docs
url: /fr/net/aspose.cells/pagesetup/order/
---
## PageSetup.Order property

Représente l'ordre que Microsoft Excel utilise pour numéroter les pages lors de l'impression d'une grande feuille de calcul.

```csharp
public PrintOrderType Order { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrderDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir l'ordre d'impression sur DownThenOver
            sheet.PageSetup.Order = PrintOrderType.DownThenOver;
            Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);

            // Enregistrez le classeur dans différents formats
            workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);

            // Modifier l'ordre d'impression en OverThenDown
            sheet.PageSetup.Order = PrintOrderType.OverThenDown;
            Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);

            // Enregistrer à nouveau avec différents formats
            workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
            workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
        }
    }
}
```

### Voir aussi

* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


