---
title: "PdfBookmarkEntry.DestinationName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PdfBookmarkEntry propriété. Obtient ou définit le nom de la destination"
type: docs
url: /fr/net/aspose.cells.rendering/pdfbookmarkentry/destinationname/
---
## PdfBookmarkEntry.DestinationName property

Obtient ou définit le nom de la destination.

```csharp
public string DestinationName { get; set; }
```

### Remarques

Si le nom de destination est défini, la destination sera définie comme une destination nommée avec ce nom.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyDestinationNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter du contenu d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Primary Content Section");
            worksheet.Cells["A2"].PutValue("Secondary Content Section");

            // Créer l'entrée principale de signet PDF
            PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
            {
                Text = "Main Section",
                Destination = worksheet.Cells["A1"],
                IsOpen = true
            };

            // Démontrer la lecture du DestinationName initial (null)
            Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");

            // Définir un nom de destination personnalisé pour l'entrée principale
            mainEntry.DestinationName = "PrimaryDestination";
            Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");

            // Créer une entrée de sous-signet
            PdfBookmarkEntry subEntry = new PdfBookmarkEntry
            {
                Text = "Sub Section",
                Destination = worksheet.Cells["A2"],
                DestinationName = "SecondaryDestination"
            };

            // Ajouter une sous-entrée au signet principal
            mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };

            // Configurer les options d'enregistrement PDF avec la structure de signets
            PdfSaveOptions pdfOptions = new PdfSaveOptions
            {
                Bookmark = mainEntry
            };

            // Enregistrer le classeur avec les signets PDF
            workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);

            Console.WriteLine("PDF created with custom bookmark destinations.");
        }
    }
}
```

### Voir aussi

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


