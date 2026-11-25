---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfBookmarkEntry. Quando questa proprietà è true la voce del segnalibro si chiuderà, altrimenti si espanderà"
type: docs
url: /it/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

Quando questa proprietà è true, il bookmarkentry si chiuderà, altrimenti si espanderà.

```csharp
public bool IsCollapse { get; set; }
```

### Esempi

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

            // Crea voce di segnalibro radice
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // Creare una sezione finanziaria chiusa
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // Aggiungere sottosezioni trimestrali alla sezione finanziaria
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // Creare una sezione operativa espansa
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // Costruire la gerarchia dei segnalibri
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // Assegnare i segnalibri alle opzioni di salvataggio
            saveOptions.Bookmark = rootEntry;

            // Salvare con i segnalibri configurati
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### Vedi anche

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


