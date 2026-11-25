---
title: "ImageConverter.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ImageConverter. Converte il file modello in immagini"
type: docs
url: /it/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Converte il file modello in immagini.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | String | Il file modello da convertire in immagini. |
| resultFile | String | Il file risultante (modello di nome) per le immagini generate. |

### Osservazioni

I file di output saranno costruiti dal file risultato specificato aggiungendo il numero di sequenza del foglio e la parte divisa. Per esempio, se il file di output specificato è Image.png, allora i file immagine generati saranno Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Esempi

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
            // Crea una nuova cartella di lavoro e popolala con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // Salva come file modello per l'elaborazione
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // Converti il modello in immagini usando i parametri (String, String)
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

### Vedi anche

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converte il file modello in immagini

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |

### Osservazioni

Durante la conversione in un'immagine di formato che supporta più pagine (come tiff), il [`OutputFile`](../../lowcodesaveoptions/outputfile/) o il [`OutputStream`](../../lowcodesaveoptions/outputstream/) specificato verrà utilizzato direttamente per l'immagine risultante. Per altri tipi di immagine, se le opzioni di salvataggio hanno specificato Stream come output, allora tutte le immagini risultanti saranno salvate nello stesso Stream. Altrimenti, i file di output saranno costruiti dal file di output specificato nelle opzioni di salvataggio aggiungendo il numero di sequenza del foglio e la parte divisa. Per esempio, se il file di output specificato è Image.png, allora i file immagine generati saranno Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Esempi

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
                // Inizializza LowCodeLoadOptions con un file modello
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // Inizializza LowCodeSaveOptions con la directory di output
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // Esegui il metodo Process con i parametri specificati
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

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Converte il file modello in immagini

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per il salvataggio. Il suo output ([`OutputFile`](../../lowcodesaveoptions/outputfile/) o [`OutputStream`](../../lowcodesaveoptions/outputstream/)) non ha effetto perché tutti gli output saranno specificati dal parametro "provider" |
| provider | AbstractLowCodeSaveOptionsProvider | Provider delle opzioni di salvataggio per salvare le immagini generate |

### Esempi

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
            
            // Crea modello di esempio
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // Inizializza le opzioni di caricamento
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // Configura le opzioni di salvataggio usando LowCodeImageSaveOptions
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // Chiama il metodo statico Process
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
                // Accedi alle proprietà di risoluzione da LowCodeImageSaveOptions
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

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


