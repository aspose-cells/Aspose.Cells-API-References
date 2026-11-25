---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore OdsLoadOptions. Rappresenta le opzioni di caricamento del file ods"
type: docs
url: /it/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

Rappresenta le opzioni di caricamento del file ODS.

```csharp
public OdsLoadOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea OdsLoadOptions usando il costruttore
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // Imposta lo stile del collegamento ipertestuale per utilizzare le impostazioni predefinite di Excel
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // Carica il file ODS con le opzioni di caricamento
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // Salva come XLSX
            workbook.Save("output.xlsx");
            
            // Verifica che lo stile del collegamento ipertestuale sia stato applicato
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### Vedi anche

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

Rappresenta le opzioni di caricamento del file ODS.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | LoadFormat | Il tipo di formato di caricamento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Crea un file ODS di esempio se non esiste
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // Crea OdsLoadOptions con il parametro LoadFormat
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // Carica la cartella di lavoro con le opzioni di caricamento create
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // Salva per dimostrare il caricamento riuscito
                    workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
                }
            }
            catch (FileNotFoundException)
            {
                Console.WriteLine("Error: Created sample file missing - please verify permissions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading ODS file: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


