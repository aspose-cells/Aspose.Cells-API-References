---
title: "TextConverter.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextConverter-metod. Konverterar given mallfil mellan textbaserade filer och andra format."
type: docs
url: /sv/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

Konverterar given mallfil mellan textbaserade filer och andra format.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | String | Mallfilen som ska konverteras |
| resultFile | String | Den resulterande filen |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class TextConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            string inputFile = "input.csv";
            string outputFile = "output.xlsx";

            // Skapa exempel CSV-fil
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // Anropa den statiska Process-metoden direkt utan att instansiera TextConverter.
                TextConverter.Process(inputFile, outputFile);
                
                Console.WriteLine($"Process method successfully converted {inputFile} to {outputFile}");
                Console.WriteLine($"Converted file exists: {File.Exists(outputFile)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            finally
            {
                // Rensa temporära filer
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### Se även

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konverterar filformat mellan textbaserade format och andra kalkylbladsfilformat

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Alternativ för indata och laddning. |
| saveOptions | LowCodeSaveOptions | Alternativ för utdata och sparning. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Skapa en exempeltextfil
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // Bearbeta textfilen med LowCode-alternativ
            using (FileStream inputStream = new FileStream(inputPath, FileMode.Open))
            {
                TextConverter.Process(
                    new LowCodeLoadOptions() { InputStream = inputStream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.txt"
                    }
                );
            }

            Console.WriteLine("Text processing completed successfully.");
        }
    }
}
```

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


