---
title: "SpreadsheetSplitter.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpreadsheetSplitter-Methode. Teilt die angegebene Vorlagendatei in mehrere Teile."
type: docs
url: /de/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Teilt die angegebene Vorlagendatei in mehrere Teile.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | String | Die zu teilende Vorlagendatei. |
| resultFile | String | Die resultierende Datei (Namensmuster). |

### Hinweise

Die Ausgabedateien werden aus der angegebenen Ergebnisdatei erstellt, indem die Sequenznummer des Blatts und des geteilten Teils angehängt wird. Zum Beispiel, wenn die angegebene Ausgabedatei Split.xlsx ist, werden die erzeugten Dateien Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Eine neue Arbeitsmappe mit mehreren Arbeitsblättern erstellen
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // Als Vorlagendatei speichern
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // Definiere das Ergebnisausgabemuster.
            string resultPattern = "SplitResult_";
            
            try
            {
                // Verarbeite die Vorlage direkt mit der statischen Methode.
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Teilt eine Tabellenkalkulationsdatei in mehrere Teile.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | LowCodeSplitOptions | Optionen zum Aufteilen von Tabellenkalkulationen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // Split-Optionen initialisieren
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // Tabellenkalkulationsteilung mit statischer Methode ausführen
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
        }
    }

    // Konkrete Implementierung von AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implementiere die erforderliche abstrakte Methode
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Siehe auch

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


