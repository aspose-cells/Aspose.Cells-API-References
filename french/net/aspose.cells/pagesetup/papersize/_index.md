---
title: "PageSetup.PaperSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la taille du papier"
type: docs
url: /fr/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Représente la taille du papier.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir la taille du papier sur Envelope B6
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // Imprimer la taille actuelle du papier
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // Enregistrez le classeur
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


