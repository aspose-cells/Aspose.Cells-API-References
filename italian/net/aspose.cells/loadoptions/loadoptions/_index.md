---
title: "LoadOptions.LoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore LoadOptions. Crea un'opzione per il caricamento del file"
type: docs
url: /it/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Crea un'opzione per il caricamento del file.

```csharp
public LoadOptions()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";

            try
            {
                // Crea contenuto CSV di esempio
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // Dimostra il costruttore predefinito
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // Dimostra il costruttore con parametro LoadFormat
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // Carica il file CSV con le opzioni specificate
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // Verifica che i dati siano stati caricati correttamente
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // Salva come XLSX per dimostrare la conversione
                workbook.Save("CsvToExcel.xlsx");
                Console.WriteLine("CSV file successfully loaded and converted to XLSX");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Crea un'opzione per il caricamento del file.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadFormat | LoadFormat | Il formato di caricamento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // Crea contenuto CSV di esempio
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // Crea LoadOptions con LoadFormat.Csv
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // Carica il file CSV con le opzioni create
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Dimostra il caricamento riuscito leggendo la cella
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Salva come XLSX per mostrare la capacità di conversione
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


