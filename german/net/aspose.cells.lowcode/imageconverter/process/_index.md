---
title: "ImageConverter.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageConverter-Methode. Konvertiert die Vorlagendatei in Bilder"
type: docs
url: /de/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Konvertiert Vorlagendateien in Bilder.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | String | Die Vorlagendatei, die in Bilder konvertiert werden soll. |
| resultFile | String | Die resultierende Datei (Namensmuster) für erzeugte Bilder. |

### Hinweise

Die Ausgabedateien werden aus der angegebenen Ergebnisdatei erstellt, indem die Sequenznummer des Blatts und des Teilsegments angehängt wird. Zum Beispiel, wenn die angegebene Ausgabedatei Image.png ist, werden die erzeugten Bilddateien Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ... sein.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch und fülle es mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // Als Vorlagendatei zum Verarbeiten speichern
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // Vorlage mit (String, String)-Parametern in Bilder konvertieren
                ImageConverter.Process("Template.xlsx", "OutputSheet.png");

                Console.WriteLine("Process method executed successfully. Generated image(s) from spreadsheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image conversion: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konvertiert Vorlagendateien in Bilder

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen für Ausgabe und Speichern |

### Hinweise

Beim Konvertieren in ein Bildformat, das mehrere Seiten unterstützt (wie TIFF), wird die angegebene [`OutputFile`](../../lowcodesaveoptions/outputfile/) oder [`OutputStream`](../../lowcodesaveoptions/outputstream/) direkt für das resultierende Bild verwendet. Für andere Bildtypen, wenn die Speicheroptionen einen Stream als Ausgabe angegeben haben, werden alle resultierenden Bilder in denselben Stream gespeichert. Andernfalls werden die Ausgabedateien aus der angegebenen Ausgabedatei der Speicheroptionen erstellt, indem die Sequenznummer des Blatts und des Teilsegments angehängt wird. Zum Beispiel, wenn die angegebene Ausgabedatei Image.png ist, werden die erzeugten Bilddateien Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ... sein.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            try
            {
                // LowCodeLoadOptions mit einer Vorlagendatei initialisieren
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // LowCodeSaveOptions mit Ausgabeverzeichnis initialisieren
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // Process-Methode mit angegebenen Parametern ausführen
                ImageConverter.Process(loadOptions, saveOptions);
                
                Console.WriteLine("Spreadsheet converted to images successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during processing: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Konvertiert Vorlagendateien in Bilder

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen zum Speichern. Seine Ausgabe ([`OutputFile`](../../lowcodesaveoptions/outputfile/) oder [`OutputStream`](../../lowcodesaveoptions/outputstream/)) hat keine Wirkung, da alle Ausgaben durch den Parameter "provider" festgelegt werden. |
| provider | AbstractLowCodeSaveOptionsProvider | Anbieter von Speicheroptionen zum Speichern der erzeugten Bilder |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
            const string templatePath = "SampleTemplate.xlsx";
            const string outputDir = "Output/";
            
            // Beispielvorlage erstellen
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // Ladeoptionen initialisieren
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // Speicheroptionen mit LowCodeImageSaveOptions konfigurieren
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // Rufen Sie die statische Process-Methode auf
                ImageConverter.Process(loadOptions, saveOptions, provider);
                Console.WriteLine($"Generated PNG images in: {Path.GetFullPath(outputDir)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Processing failed: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string path)
        {
            using (Workbook wb = new Workbook())
            {
                Worksheet sheet = wb.Worksheets[0];
                sheet.Cells["A1"].PutValue("LowCode Process Demo");
                sheet.Cells["B3"].PutValue(DateTime.Now.ToString());
                wb.Save(path, SaveFormat.Xlsx);
            }
        }

        private class DynamicSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            private readonly LowCodeImageSaveOptions _baseOptions; // Corrected type

            public DynamicSaveOptionsProvider(LowCodeImageSaveOptions options)
            {
                _baseOptions = options;
            }

            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Zugriff auf Auflösungseigenschaften von LowCodeImageSaveOptions
                if (partInfo.SheetIndex == 0)
                {
                    _baseOptions.ImageOptions.HorizontalResolution = 300;
                    _baseOptions.ImageOptions.VerticalResolution = 300;
                }
                return _baseOptions;
            }
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


