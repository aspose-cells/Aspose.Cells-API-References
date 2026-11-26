---
title: "Clase PdfBookmarkEntry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.PdfBookmarkEntry. PdfBookmarkEntry es una entrada en el marcador PDF. si la propiedad Text de la instancia actual es nula o la instancia actual será oculta y los hijos se insertarán en el nivel actual"
type: docs
url: /es/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry es una entrada en el marcador PDF. Si la propiedad Text de la instancia actual es nula o "", la instancia actual se ocultará y los hijos se insertarán en el nivel actual.

```csharp
public class PdfBookmarkEntry
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | La celda a la que enlaza el marcador. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Obtiene o establece el nombre del destino. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | Cuando esta propiedad es verdadera, la bookmarkentry se colapsará, de lo contrario se expandirá. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | Cuando esta propiedad es verdadera, la bookmarkentry se expandirá, de lo contrario se colapsará. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | SubEntry de un marcador. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Título de un marcador. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo y agregar hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Obtener celdas de cada hoja de cálculo
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // Colocar valores en las celdas
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // Crear el PdfBookmarkEntry raíz
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Crear sub PdfBookmarkEntries
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

            // Agregar subentradas a la entrada raíz
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // Crear PdfSaveOptions y establecer el marcador
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // Guardar el libro de trabajo como PDF con marcadores
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


