---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt den Ausgabedateiformattyp zurück oder legt ihn fest. Unterstützt Tiff/XPS."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

Gibt den Ausgabedateiformattyp zurück oder legt ihn fest. Unterstützt Tiff/XPS.

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen für Tiff/Svg [`ImageType`](../imagetype/); für Xps [`Save`](../../../aspose.cells/workbook/save/) mit [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). Diese Eigenschaft wird 12 Monate später, seit August 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und fülle Beispieldaten ein
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // Erstelle eine ImageOrPrintOptions-Instanz
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Anfangswert von SaveFormat anzeigen
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Setze SaveFormat auf TIFF und rendere das Arbeitsblatt
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // Ändere SaveFormat zu XPS und rendere erneut
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // Hinweis: SheetRender unterstützt das XPS-Format nicht. Stattdessen wird es als Bildformat gespeichert.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


