---
title: "PdfSaveOptions.PdfCompression"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Indique l'algorithme de compression"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Indique l'algorithme de compression

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyPdfCompressionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample PDF Compression Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfCompression property usage");
            
            // Créer des options d'enregistrement PDF avec compression Flate
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PdfCompression = PdfCompressionCore.Flate;
            
            // Enregistrer le classeur au format PDF avec compression
            workbook.Save("output_with_flate_compression.pdf", saveOptions);
            
            // Enregistrez à nouveau sans compression pour la comparaison
            saveOptions.PdfCompression = PdfCompressionCore.None;
            workbook.Save("output_without_compression.pdf", saveOptions);
            
            Console.WriteLine("PDF files created successfully with different compression settings.");
        }
    }
}
```

### Voir aussi

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


