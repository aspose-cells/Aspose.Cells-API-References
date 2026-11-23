---
title: "PdfBookmarkEntry.Destination"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PdfBookmarkEntry propriété. La cellule vers laquelle le lien du signet"
type: docs
url: /fr/net/aspose.cells.rendering/pdfbookmarkentry/destination/
---
## PdfBookmarkEntry.Destination property

La cellule vers laquelle le lien du signet pointe.

```csharp
public Cell Destination { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyDestinationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du contenu d'exemple
            worksheet.Cells["A1"].PutValue("Bookmark Destination");
            
            // Configurer les options d'enregistrement PDF avec le signet
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Sample Bookmark";
            entry.Destination = worksheet.Cells["A1"]; // Demonstrate Destination property
            entry.IsOpen = true;
            
            pdfSaveOptions.Bookmark = entry;
            
            // Enregistrer le PDF
            workbook.Save("PdfBookmarkEntryPropertyDestinationDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


