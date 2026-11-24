---
title: "ImageOrPrintOptions.EmfType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions‑Eigenschaft. Gibt einen EmfType zurück oder legt ihn fest, der das Format der Metadatei angibt. Der Standardwert ist EmfPlusDual"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Ruft einen EmfType ab oder legt ihn fest, der das Format der Metafile angibt. Der Standardwert ist EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // Erstelle eine ImageOrPrintOptions-Instanz
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Bildtyp auf EMF setzen
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // SheetRender mit den Optionen erstellen
                SheetRender renderer = new SheetRender(worksheet, options);

                // Im EMF-Format speichern
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // Den Wert der EmfType‑Eigenschaft anzeigen
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // Speichern Sie die EMF-Datei
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


