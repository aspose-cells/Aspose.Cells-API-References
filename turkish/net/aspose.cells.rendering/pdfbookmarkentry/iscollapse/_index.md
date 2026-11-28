---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfBookmarkEntry özelliği. Bu özellik true olduğunda yer imi girişi daralır, aksi takdirde genişler"
type: docs
url: /tr/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

Bu özellik true olduğunda, bookmarkentry daralır, aksi takdirde genişler.

```csharp
public bool IsCollapse { get; set; }
```

### Örnekler

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

            // Kök yer imi girdisi oluşturun
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // Katlanmış finansal bölümü oluştur
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // Finansal bölüme üç aylık alt bölümler ekle
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // Genişletilmiş operasyonel bölümü oluştur
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // Yer imi hiyerarşisini oluştur
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // Yer imlerini kaydetme seçeneklerine ata
            saveOptions.Bookmark = rootEntry;

            // Yapılandırılmış yer imleriyle kaydet
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


