---
title: "SpreadsheetMerger.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpreadsheetMerger Methode. Zusammenführen der angegebenen Vorlagendateien"
type: docs
url: /de/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

Führe die angegebenen Vorlagendateien zusammen.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFiles | String[] | Die zu zusammenführenden Vorlagendateien |
| resultFile | String | Die resultierende Datei |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithStringArrayStringDemo
    {
        public static void Run()
        {
            // Erstelle Beispiel-Vorlagendateien
            CreateTemplateFile("template1.xlsx", "Data from Template 1");
            CreateTemplateFile("template2.xlsx", "Data from Template 2");

            string[] templateFiles = { "template1.xlsx", "template2.xlsx" };
            string resultFile = "merged_output.xlsx";

            try
            {
                SpreadsheetMerger.Process(templateFiles, resultFile);

                Console.WriteLine($"Process method merged {templateFiles.Length} files into {resultFile}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Siehe auch

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

Führt mehrere Vorlagendateien zu einer zusammen.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | LowCodeMergeOptions | Optionen zum Zusammenführen von Dateien |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithLowCodeMergeOptDemo
    {
        public static void Run()
        {
            // Bereite zwei einfache Vorlagendateien vor, die zusammengeführt werden.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // Erstelle eine Instanz der Optionsklasse.
                // Die LowCodeMergeOptions-Klasse ist Teil von Aspose.Cells.LowCode.
                // Für diese Demo verwenden wir den Standardkonstruktor.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // Rufen Sie die Process-Methode auf, die LowCodeMergeOptions akzeptiert.
                SpreadsheetMerger.Process(options);

                Console.WriteLine("Process method invoked successfully with LowCodeMergeOptions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Siehe auch

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


