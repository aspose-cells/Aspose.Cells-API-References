---
title: "TextConverter.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextConverter-Methode. Konvertiert die angegebene Vorlagendatei zwischen textbasierten Dateien und anderen Formaten"
type: docs
url: /de/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

Konvertiert die angegebene Vorlagendatei zwischen textbasierten Dateien und anderen Formaten.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | String | Die zu konvertierende Vorlagendatei |
| resultFile | String | Die resultierende Datei |

### Beispiele

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

            // Erstelle Beispiel-CSV-Datei
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // Rufen Sie die statische Process-Methode direkt auf, ohne TextConverter zu instanziieren
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
                // Bereinige temporäre Dateien
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### Siehe auch

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konvertiert das Dateiformat zwischen textbasierten Formaten und anderen Tabellenkalkulationsdateiformaten

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen für Ausgabe und Speichern |

### Beispiele

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
            // Erstellen Sie eine Beispiel-Textdatei
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // Verarbeite die Textdatei mit LowCode-Optionen
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

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


