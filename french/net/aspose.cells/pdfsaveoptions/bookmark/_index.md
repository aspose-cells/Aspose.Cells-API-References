---
title: "PdfSaveOptions.Bookmark"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Obtient et définit l’objet PdfBookmarkEntry"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

Obtient et définit l’objet [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/).

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyBookmarkDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter trois feuilles de calcul
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");

            // Définissez les valeurs dans les cellules qui seront des destinations de signet
            sheet1.Cells["A1"].Value = "Sheet1 Content";
            sheet2.Cells["A1"].Value = "Sheet2 Content";
            sheet3.Cells["A1"].Value = "Sheet3 Content";

            // Créer le signet racine
            PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
            {
                Text = "Root",
                Destination = sheet1.Cells["A1"],
                IsOpen = true
            };

            // Créer des sous‑signets
            PdfBookmarkEntry subBookmark1 = new PdfBookmarkEntry
            {
                Text = "Sheet2",
                Destination = sheet2.Cells["A1"]
            };

            PdfBookmarkEntry subBookmark2 = new PdfBookmarkEntry
            {
                Text = "Sheet3",
                Destination = sheet3.Cells["A1"]
            };

            // Ajouter des sous‑signets à la racine
            rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };

            // Configurer les options d’enregistrement PDF avec des signets
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = rootBookmark
            };

            // Enregistrer dans un flux mémoire (peut être enregistré dans un fichier en utilisation réelle)
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Voir aussi

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


