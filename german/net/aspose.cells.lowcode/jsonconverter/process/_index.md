---
title: "JsonConverter.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "JsonConverter-Methode. Konvertiert die angegebene Vorlagendatei zwischen json und anderen Formaten"
type: docs
url: /de/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

Konvertiert die angegebene Vorlagendatei zwischen JSON und anderen Formaten.

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

    public class JsonConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle Beispiel-JSON-Daten und schreibe sie in eine temporäre Datei
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // Verarbeite Dateien direkt mit der statischen Methode von JsonConverter
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // Bereinige die temporäre JSON-Datei
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Siehe auch

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konvertiert zwischen JSON-Daten und anderen Tabellenkalkulationsdateiformaten.

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
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class JsonConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Beispieldaten für JSON erstellen
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // Erstelle einen Memory-Stream mit den JSON-Daten
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // Verarbeite die JSON-Daten mit LowCode-Optionen
                JsonConverter.Process(
                    new LowCodeLoadOptions() { InputStream = stream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.json"
                    });
            }

            Console.WriteLine("JSON processing completed successfully.");
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


