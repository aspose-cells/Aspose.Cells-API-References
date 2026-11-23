---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Si PrintWithStatusDialog true, une boîte de dialogue affichera l'état d'impression actuel. Sinon, aucune boîte de dialogue ne sera affichée."
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera affichée. Sinon, aucune boîte de dialogue ne sera affichée.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // Initialiser un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Définir les options d’image ou d’impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // Créer un rendu de feuille
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // Imprimer en PDF
            sheetRender.ToImage(0, "output.png");

            // Attendre la création du fichier (logique d'attente simplifiée)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


