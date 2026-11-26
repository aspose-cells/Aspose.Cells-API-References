---
title: "PdfBookmarkEntry.DestinationName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfBookmarkEntry. Obtiene o establece el nombre del destino"
type: docs
url: /es/net/aspose.cells.rendering/pdfbookmarkentry/destinationname/
---
## PdfBookmarkEntry.DestinationName property

Obtiene o establece el nombre del destino.

```csharp
public string DestinationName { get; set; }
```

### Observaciones

Si se establece el nombre del destino, el destino se definirá como un destino nombrado con este nombre.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyDestinationNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar contenido de ejemplo a las celdas
            worksheet.Cells["A1"].PutValue("Primary Content Section");
            worksheet.Cells["A2"].PutValue("Secondary Content Section");

            // Crear entrada principal de marcador PDF
            PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
            {
                Text = "Main Section",
                Destination = worksheet.Cells["A1"],
                IsOpen = true
            };

            // Demostrar la lectura del DestinationName inicial (null)
            Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");

            // Establecer un nombre de destino personalizado para la entrada principal
            mainEntry.DestinationName = "PrimaryDestination";
            Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");

            // Crear una entrada de submarcador
            PdfBookmarkEntry subEntry = new PdfBookmarkEntry
            {
                Text = "Sub Section",
                Destination = worksheet.Cells["A2"],
                DestinationName = "SecondaryDestination"
            };

            // Agregar una subentrada al marcador principal
            mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };

            // Configurar las opciones de guardado PDF con la estructura de marcadores
            PdfSaveOptions pdfOptions = new PdfSaveOptions
            {
                Bookmark = mainEntry
            };

            // Guardar el libro de trabajo con marcadores PDF
            workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);

            Console.WriteLine("PDF created with custom bookmark destinations.");
        }
    }
}
```

### Ver también

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


