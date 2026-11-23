---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfBookmarkEntry. Lorsque cette propriété est vraie, l'entrée de signet se repliera sinon elle s'étendra"
type: docs
url: /fr/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

Lorsque cette propriété est vraie, le bookmarkentry se repliera, sinon il s'étendra.

```csharp
public bool IsCollapse { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyIsCollapseDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Créer une entrée de signet racine
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // Créer une section financière repliée
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // Ajouter des sous-sections trimestrielles à la section financière
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // Créer une section opérationnelle développée
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // Construire la hiérarchie des signets
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // Attribuer les signets aux options d'enregistrement
            saveOptions.Bookmark = rootEntry;

            // Enregistrer avec les signets configurés
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### Voir aussi

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


