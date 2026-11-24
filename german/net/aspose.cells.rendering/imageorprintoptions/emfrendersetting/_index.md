---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Einstellung zum Rendern von Emf-Metadateien in der Quelldatei"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Einstellung zum Rendern von EMF-Metadateien in der Quelldatei.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Hinweise

EMF-Metadateien, die als "EMF+ Dual" identifiziert werden, können sowohl EMF+-Datensätze als auch EMF-Datensätze enthalten. Jeder Datensatztyp kann zum Rendern des Bildes verwendet werden, nur EMF+-Datensätze oder nur EMF-Datensätze. Wenn EmfPlusPrefer gesetzt ist, werden beim Rendern zum Bild EMF+-Datensätze geparst, andernfalls werden nur EMF-Datensätze geparst. Der Standardwert ist EmfOnly. Für Frameworks, die von .NET System.Drawing.Common abhängen, wird diese Einstellung ignoriert.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Testinhalt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // Bildrenderoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // Aktuelle Einstellung anzeigen
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // Mit den Standard-EMF-Einstellungen rendern
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // EMF-Render-Einstellung ändern und erneut rendern
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### Siehe auch

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


