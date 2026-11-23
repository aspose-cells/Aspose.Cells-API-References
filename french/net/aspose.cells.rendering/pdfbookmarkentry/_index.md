---
title: "Classe PdfBookmarkEntry"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.PdfBookmarkEntry. PdfBookmarkEntry est une entrée dans le signet PDF. si la propriété Text de l'instance actuelle est nulle ou l'instance actuelle sera masquée et les enfants seront insérés au même niveau"
type: docs
url: /fr/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry est une entrée dans le signet PDF. Si la propriété Text de l'instance actuelle est null ou \"\", l'instance actuelle sera masquée et les enfants seront insérés au même niveau.

```csharp
public class PdfBookmarkEntry
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | La cellule vers laquelle le lien du signet pointe. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Obtient ou définit le nom de la destination. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | Lorsque cette propriété est vraie, le bookmarkentry se repliera, sinon il s'étendra. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | Lorsque cette propriété est vraie, le bookmarkentry s'étendra, sinon il se repliera. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | SubEntry d'un signet. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Titre d'un signet. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Collections;

    public class PdfBookmarkEntryDemo
    {
        public static void PdfBookmarkEntryExample()
        {
            // Créer un nouveau classeur et ajouter des feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Obtenir les cellules de chaque feuille de calcul
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // Insérer des valeurs dans les cellules
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // Créer le PdfBookmarkEntry racine
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Créer des PdfBookmarkEntries secondaires
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
            {
                Text = "section1",
                Destination = cellInPage2
            };

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
            {
                Text = "section2",
                Destination = cellInPage3
            };

            // Ajouter des sous-entrées à l'entrée racine
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // Créer PdfSaveOptions et définir le signet
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // Enregistrer le classeur au format PDF avec des signets
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


