---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfBookmarkEntry-Eigenschaft. Wenn diese Eigenschaft wahr ist, wird der Lesezeicheneintrag zusammengeklappt, andernfalls wird er erweitert."
type: docs
url: /de/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

Wenn diese Eigenschaft true ist, wird das bookmarkentry zusammengeklappt, andernfalls wird es erweitert.

```csharp
public bool IsCollapse { get; set; }
```

### Beispiele

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

            // Root-Lesezeicheneintrag erstellen
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // Zusammengeklappten Finanzabschnitt erstellen
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // Quartalsunterabschnitte zum Finanzabschnitt hinzufügen
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // Erweiterten Betriebsabschnitt erstellen
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // Lesezeichenhierarchie erstellen
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // Lesezeichen den Speicheroptionen zuweisen
            saveOptions.Bookmark = rootEntry;

            // Mit konfigurierten Lesezeichen speichern
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### Siehe auch

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


