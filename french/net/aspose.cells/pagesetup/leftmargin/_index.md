---
title: "PageSetup.LeftMargin"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la taille de la marge gauche en centimètres"
type: docs
url: /fr/net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Représente la taille de la marge gauche, en centimètres.

```csharp
public double LeftMargin { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir des données d'exemple
            sheet.Cells["A1"].PutValue("Left Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows how to set page margins");

            // Définir la marge gauche (en pouces)
            sheet.PageSetup.LeftMargin = 1.5;

            // Imprimez la valeur de la marge gauche dans la console
            Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");

            // Enregistrez en PDF pour démontrer la marge
            string outputPath = "LeftMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("File saved with left margin: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


