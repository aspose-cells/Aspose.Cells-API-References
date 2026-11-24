---
title: "ConversionUtility.Convert"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConversionUtility-Methode. Konvertiert Excel-Dateien in andere Formate"
type: docs
url: /de/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Konvertiert Excel-Dateien in andere Formate.

```csharp
public static void Convert(string source, string saveAs)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | String | Der Quelldateiname. |
| saveAs | String | Der Dateiname der erwarteten Datei. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ConversionUtilityMethodConvertWithStringStringDemo
    {
        public static void Run()
        {
            // Quell‑ und Zielpfade initialisieren
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // Excel-Datei in PDF konvertieren
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Siehe auch

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Konvertiert Excel-Dateien in andere Formate.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | String | Der Quelldateiname. |
| loadOptions | LoadOptions | Die Optionen zum Laden der Quelldatei. |
| saveAs | String | Der Dateiname der erwarteten Datei. |
| saveOptions | SaveOptions | Die Optionen zum Speichern der Datei. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
    {
        public static void Run()
        {
            // Quell‑ und Zielpfade
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // Beispiel-CSV-Datei zur Demonstration erstellen
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // Ladeoptionen für CSV-Datei erstellen
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // Speicheroptionen für XLSX-Datei erstellen
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // CSV in XLSX mit angegebenen Optionen konvertieren
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // Überprüfen Sie die Konvertierung, indem Sie die Ausgabedatei laden
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Bereinige temporäre Dateien
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


