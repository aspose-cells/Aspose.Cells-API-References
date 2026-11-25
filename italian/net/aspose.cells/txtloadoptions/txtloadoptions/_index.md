---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore TxtLoadOptions. Crea le opzioni per il caricamento del file di testo"
type: docs
url: /it/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Crea le opzioni per il caricamento di un file di testo.

```csharp
public TxtLoadOptions()
```

### Osservazioni

Il tipo di file di caricamento predefinito è CSV .

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo TxtLoadOptions usando il costruttore
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // Imposta il separatore per il file CSV
            loadOptions.Separator = ',';
            
            // Crea una cartella di lavoro con le opzioni di caricamento
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Emetti alcune informazioni dal file caricato
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Crea le opzioni per il caricamento di un file di testo.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadFormat | LoadFormat | Il formato di caricamento |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Crea contenuto CSV di esempio e file temporaneo
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // Crea TxtLoadOptions con LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Carica CSV usando le opzioni configurate
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Dimostra i dati caricati
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // Salva la cartella di lavoro elaborata
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Pulisci il file temporaneo
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


