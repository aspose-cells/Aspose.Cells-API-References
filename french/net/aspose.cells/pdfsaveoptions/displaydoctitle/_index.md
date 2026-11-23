---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Indique si la barre de titre de Windows doit afficher le titre du document"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Indique si la barre de titre de la fenêtre doit afficher le titre du document.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Remarques

Si false, la barre de titre doit afficher le nom du fichier PDF à la place. La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyDisplayDocTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // Créez les options d'enregistrement PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Définissez la propriété DisplayDocTitle sur true
            pdfSaveOptions.DisplayDocTitle = true;

            // Enregistrez le classeur au format PDF
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


