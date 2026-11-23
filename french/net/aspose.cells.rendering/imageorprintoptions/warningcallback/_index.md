---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit le rappel d'avertissement"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

Obtient ou définit le rappel d'avertissement.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter du contenu qui générera un avertissement lors du rendu
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // Créer une instance de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Afficher la valeur initiale de WarningCallback
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // Créer et assigner un rappel d'avertissement personnalisé
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // Créer SheetRender pour démontrer le rappel pendant le rendu
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // Vérifier si les avertissements ont été capturés
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // Implémentation de rappel personnalisée pour gérer les avertissements de rendu
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // Gérer les avertissements de substitution de police
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### Voir aussi

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


