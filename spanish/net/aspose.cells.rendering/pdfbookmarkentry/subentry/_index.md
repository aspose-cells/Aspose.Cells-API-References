---
title: "PdfBookmarkEntry.SubEntry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfBookmarkEntry. Subentrada de un marcador"
type: docs
url: /es/net/aspose.cells.rendering/pdfbookmarkentry/subentry/
---
## PdfBookmarkEntry.SubEntry property

SubEntry de un marcador.

```csharp
public ArrayList SubEntry { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertySubEntryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Crear entrada de marcador raíz
            PdfBookmarkEntry root = new PdfBookmarkEntry
            {
                Text = "Main Bookmark",
                Destination = workbook.Worksheets[0].Cells["A1"],
                SubEntry = new ArrayList(),
                IsOpen = true
            };

            // Crear submarcadores
            PdfBookmarkEntry sub1 = new PdfBookmarkEntry
            {
                Text = "First Section",
                Destination = workbook.Worksheets[1].Cells["A1"]
            };

            PdfBookmarkEntry sub2 = new PdfBookmarkEntry
            {
                Text = "Second Section",
                Destination = workbook.Worksheets[2].Cells["A1"],
                SubEntry = new ArrayList()
            };

            // Agregar submarcador anidado
            PdfBookmarkEntry subSub = new PdfBookmarkEntry
            {
                Text = "Sub-Section",
                Destination = workbook.Worksheets[2].Cells["B1"]
            };
            sub2.SubEntry.Add(subSub);

            // Agregar submarcadores a la raíz
            root.SubEntry.Add(sub1);
            root.SubEntry.Add(sub2);

            // Guardar con marcadores
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = root
            };
            workbook.Save("output_with_bookmarks.pdf", options);
        }
    }
}
```

### Ver también

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


