---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfBookmarkEntry-egenskap. När denna egenskap är sann kommer bokmärkesposten att kollapsa, annars expandera"
type: docs
url: /sv/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

När denna egenskap är sann kommer bookmarkentry att kollapsa, annars expanderar den.

```csharp
public bool IsCollapse { get; set; }
```

### Exempel

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

            // Skapa rotbokmärkespost
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // Skapa kollapsad finansiell sektion
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // Lägg till kvartalsvisa underavsnitt i den finansiella sektionen
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // Skapa en utökad operativ sektion
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // Bygg bokmärkeshierarki
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // Tilldela bokmärken till sparaalternativ
            saveOptions.Bookmark = rootEntry;

            // Spara med konfigurerade bokmärken
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### Se även

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


