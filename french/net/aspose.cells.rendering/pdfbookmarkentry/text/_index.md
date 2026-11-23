---
title: "PdfBookmarkEntry.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PdfBookmarkEntry propriété. Titre d'un signet"
type: docs
url: /fr/net/aspose.cells.rendering/pdfbookmarkentry/text/
---
## PdfBookmarkEntry.Text property

Titre d'un signet.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du contenu d'exemple
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Créer une entrée de signet PDF
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Section 1"; // Demonstrating Text property usage
            entry.Destination = worksheet.Cells["A1"];
            entry.IsOpen = true;
            
            // Définir les options d'enregistrement avec le signet
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.Bookmark = entry;
            
            // Enregistrer le classeur avec le signet
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF with bookmark created successfully.");
        }
    }
}
```

### Voir aussi

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


