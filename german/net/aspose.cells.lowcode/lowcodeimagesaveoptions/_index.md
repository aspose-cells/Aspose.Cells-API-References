---
title: "Klasse LowCodeImageSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodeImageSaveOptions Klasse. Optionen zum Speichern von Bildern auf Low‑Code‑Weise"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

Optionen zum Speichern von Bildern in Low‑Code‑Manier.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | Die Optionen zum Rendern von Bildern. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Liest und schreibt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird [`OutputStream`](../lowcodesaveoptions/outputstream/) ignoriert. (Geerbt von [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Liest und schreibt den Stream, in den die erzeugten Daten geschrieben werden. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird [`OutputFile`](../lowcodesaveoptions/outputfile/) ignoriert. (Geerbt von [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | Liest oder setzt das Speicherformat. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | Anbieter von Speicheroptionen zum Speichern generierter Bilder. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Beispieldaten zum Arbeitsblatt hinzufügen
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // Erstelle eine Instanz von LowCodeImageSaveOptions
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // Grundlegende Eigenschaften festlegen
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // Aktuelle Einstellungen anzeigen
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // Einige Bildoptionen ändern
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // Einfachen Speicheroptionsanbieter erstellen
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // Arbeitsblatt als Bild speichern
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


