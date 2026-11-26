---
title: "PdfSaveOptions.Bookmark"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene y establece el objeto PdfBookmarkEntry"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/bookmark/
---
## PdfSaveOptions.Bookmark property

Obtiene y establece el objeto [`PdfBookmarkEntry`](../../../aspose.cells.rendering/pdfbookmarkentry/).

```csharp
public PdfBookmarkEntry Bookmark { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar tres hojas de cálculo
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            Worksheet sheet3 = workbook.Worksheets.Add("Sheet3");

            // Establezca valores en celdas que serán destinos de marcadores
            sheet1.Cells["A1"].Value = "Sheet1 Content";
            sheet2.Cells["A1"].Value = "Sheet2 Content";
            sheet3.Cells["A1"].Value = "Sheet3 Content";

            // Crear marcador raíz
            PdfBookmarkEntry rootBookmark = new PdfBookmarkEntry
            {
                Text = "Root",
                Destination = sheet1.Cells["A1"],
                IsOpen = true
            };

            // Crear submarcadores
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

            // Agregar submarcadores a la raíz
            rootBookmark.SubEntry = new ArrayList { subBookmark1, subBookmark2 };

            // Configurar opciones de guardado PDF con marcadores
            PdfSaveOptions options = new PdfSaveOptions
            {
                Bookmark = rootBookmark
            };

            // Guardar en flujo de memoria (podría guardarse en un archivo en uso real)
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Ver también

* class [PdfBookmarkEntry](../../../aspose.cells.rendering/pdfbookmarkentry/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


