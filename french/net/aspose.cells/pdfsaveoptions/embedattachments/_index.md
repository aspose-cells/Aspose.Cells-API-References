---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Indique si l'attachement doit être intégré pour les objets Ole dans Excel"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

Indique s'il faut intégrer les pièces jointes pour les objets Ole dans Excel.

```csharp
public bool EmbedAttachments { get; set; }
```

### Remarques

La valeur par défaut est false. La valeur doit être false lorsque la conformité PDF/A est définie ou que le chiffrement PDF est activé.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
using System.IO;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedAttachmentsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // Créez un fichier d'exemple à intégrer
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // Ajoutez une pièce jointe (objet OLE) à la feuille de calcul
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // Créez les options d'enregistrement PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Définissez la propriété EmbedAttachments sur true
            pdfSaveOptions.EmbedAttachments = true;

            // Enregistrez le classeur au format PDF avec des pièces jointes intégrées
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // Nettoyer
            File.Delete(sampleFile);
        }
    }
}
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


