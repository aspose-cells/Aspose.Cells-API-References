---
title: "PdfBookmarkEntry.IsOpen"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfBookmarkEntry. Когда это свойство истинно, запись закладки будет развёрнута, иначе будет свернута."
type: docs
url: /ru/net/aspose.cells.rendering/pdfbookmarkentry/isopen/
---
## PdfBookmarkEntry.IsOpen property

Если это свойство истинно, bookmarkentry будет развернут, иначе он будет свернут.

```csharp
public bool IsOpen { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyIsOpenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Root";
            rootEntry.Destination = workbook.Worksheets[0].Cells["A1"];
            rootEntry.IsOpen = false; // Demonstrating IsOpen property - bookmarks will be collapsed by default
            
            PdfBookmarkEntry childEntry1 = new PdfBookmarkEntry();
            childEntry1.Text = "Child 1";
            childEntry1.Destination = workbook.Worksheets[0].Cells["B1"];
            
            PdfBookmarkEntry childEntry2 = new PdfBookmarkEntry();
            childEntry2.Text = "Child 2";
            childEntry2.Destination = workbook.Worksheets[1].Cells["A1"];
            
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(childEntry1);
            rootEntry.SubEntry.Add(childEntry2);

            PdfSaveOptions options = new PdfSaveOptions();
            options.Bookmark = rootEntry;
            
            workbook.Save("output.pdf", options);
        }
    }
}
```

### См. также

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


