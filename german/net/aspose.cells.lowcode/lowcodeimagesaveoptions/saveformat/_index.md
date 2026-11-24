---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeImageSaveOptions-Eigenschaft. Gibt das Speicherformat zurück oder legt es fest"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

Liest oder setzt das Speicherformat.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Hinweise

Wenn [`ImageOptions`](../imageoptions/) angegeben wurde, ändert das Festlegen dieser Eigenschaft auch den [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/)-Wert davon.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // LowCodeImageSaveOptions mit Standardwerten initialisieren
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // Anfängliches SaveFormat anzeigen (Standard ist Png)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Für JPEG-Ausgabe konfigurieren
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // Auf PNG-Format umstellen und erneut speichern
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // Arbeitsblatt mit den konfigurierten Optionen rendern
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


