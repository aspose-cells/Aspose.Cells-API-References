---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeImageSaveOptions-Eigenschaft. Anbieter von Speicheroptionen zum Speichern generierter Bilder"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

Anbieter von Speicheroptionen zum Speichern generierter Bilder.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Hinweise

Die Ausgabe([`OutputFile`](../../lowcodesaveoptions/outputfile/) oder [`OutputStream`](../../lowcodesaveoptions/outputstream/)), die von dieser Instanz angegeben wird, hat keine Wirkung, wenn diese Eigenschaft festgelegt ist. Stattdessen wird die Ausgabe jedes erzeugten Bildes vom Provider angegeben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // LowCodeImageSaveOptions-Instanz erstellen
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // Benutzerdefinierten SaveOptionsProvider erstellen
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // Aktuellen SaveOptionsProvider anzeigen
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // Effekt demonstrieren, indem mit verschiedenen Optionen gespeichert wird
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // Auf Null-Provider wechseln
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Benutzerdefinierte Speicheroptionen für jeden Teil zurückgeben
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Führen Sie nach dem Speichern alle Aufräumarbeiten durch
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### Siehe auch

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


