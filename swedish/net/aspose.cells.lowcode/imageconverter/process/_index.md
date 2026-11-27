---
title: "ImageConverter.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageConverter-metod. Konverterar mallfil till bilder"
type: docs
url: /sv/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Konverterar mallfil till bilder.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | String | Mallfilen som ska konverteras till bilder. |
| resultFile | String | Den resulterande filen (namnmönster) för genererade bilder. |

### Anmärkningar

Utdatafilerna kommer att byggas från den angivna resultatfilen genom att lägga till sekvensnummer för bladet och delningsdelen. Till exempel, om den angivna utdatafilen är Image.png, kommer de genererade bildfilerna att vara Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Exempel

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
            // Skapa en ny arbetsbok och fyll den med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // Spara som mallfil för bearbetning
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // Konvertera mall till bilder med (String, String)-parametrar
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

### Se även

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konverterar mallfil till bilder

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för utdata och sparning. |

### Anmärkningar

När du konverterar till en bild i ett format som stöder flera sidor (t.ex. tiff) kommer den angivna [`OutputFile`](../../lowcodesaveoptions/outputfile/) eller [`OutputStream`](../../lowcodesaveoptions/outputstream/) att användas direkt för den resulterande bilden. För andra bildtyper, om sparalternativen har specificerat Stream som utdata, kommer alla resulterande bilder att sparas till samma Stream. Annars kommer utdatafilerna att byggas från den angivna utdatafilen i sparalternativen genom att lägga till sekvensnummer för bladet och delningsdelen. Till exempel, om den angivna utdatafilen är Image.png, kommer de genererade bildfilerna att vara Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Exempel

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
                // Initiera LowCodeLoadOptions med en mallfil
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // Initiera LowCodeSaveOptions med utdata-katalog
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // Utför Process-metoden med angivna parametrar
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

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Konverterar mallfil till bilder

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för sparande. Dess utdata ([`OutputFile`](../../lowcodesaveoptions/outputfile/) eller [`OutputStream`](../../lowcodesaveoptions/outputstream/)) har ingen effekt eftersom alla utdata kommer att specificeras av parametern "provider". |
| leverantör | AbstractLowCodeSaveOptionsProvider | Leverantör av sparalternativ för att spara de genererade bilderna |

### Exempel

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
            
            // Skapa exempelmall
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // Initiera laddningsalternativ
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // Konfigurera sparalternativ med LowCodeImageSaveOptions
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // Anropa statisk Process-metod
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
                // Få åtkomst till upplösningsegenskaper från LowCodeImageSaveOptions
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

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


