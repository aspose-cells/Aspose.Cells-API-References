---
title: "SpreadsheetMerger.Process"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpreadsheetMerger-metod. Slå samman angivna mallfiler"
type: docs
url: /sv/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

Slå samman angivna mallfiler.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFiles | String[] | Mallfilerna som ska slås samman |
| resultFile | String | Den resulterande filen |

### Exempel

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
            // Skapa exempelmallfiler
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

### Se även

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

Slår samman flera mallfiler till en.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | LowCodeMergeOptions | Alternativ för att slå samman filer |

### Exempel

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
            // Förbered två enkla mallfiler som ska slås samman.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // Skapa en instans av alternativklassen.
                // LowCodeMergeOptions‑klassen är en del av Aspose.Cells.LowCode.
                // För den här demonstrationen använder vi standardkonstruktorn.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // Anropa Process‑metoden som accepterar LowCodeMergeOptions.
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

### Se även

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


