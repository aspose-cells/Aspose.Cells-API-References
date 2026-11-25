---
title: "SpreadsheetMerger.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SpreadsheetMerger metodo. Unisci i file modello forniti"
type: docs
url: /it/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

Unisci i file modello forniti.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFiles | String[] | I file modello da unire |
| resultFile | String | Il file risultante |

### Esempi

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
            // Crea file modello di esempio
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

### Vedi anche

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

Unisce più file modello in uno solo.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | LowCodeMergeOptions | Opzioni per l'unione dei file |

### Esempi

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
            // Prepara due semplici file modello che saranno uniti.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // Crea un'istanza della classe delle opzioni.
                // La classe LowCodeMergeOptions fa parte di Aspose.Cells.LowCode.
                // Per questa demo utilizziamo il costruttore predefinito.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // Chiama il metodo Process che accetta LowCodeMergeOptions.
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

### Vedi anche

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


