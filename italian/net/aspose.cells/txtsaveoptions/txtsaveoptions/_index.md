---
title: "TxtSaveOptions.TxtSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore TxtSaveOptions. Crea le opzioni di salvataggio per file di testo"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/txtsaveoptions/
---
## TxtSaveOptions() {#constructor}

Crea le opzioni di salvataggio del file di testo.

```csharp
public TxtSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Dimostra il costruttore TxtSaveOptions
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.SeparatorString = "|";
            
            // Salva con separatore personalizzato
            workbook.Save("output.txt", txtSaveOptions);
            
            Console.WriteLine("File saved with custom separator successfully.");
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni di salvataggio del file di testo.

```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato del file. Deve essere Csv o Tsv, altrimenti il formato salvato verrà impostato automaticamente su Csv. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Chiama il metodo #ctor con il parametro SaveFormat
                TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
                
                // Configura le opzioni di salvataggio
                saveOptions.Separator = ',';
                saveOptions.Encoding = Encoding.UTF8;
                saveOptions.QuoteType = TxtValueQuoteType.Always;
                
                Console.WriteLine("TxtSaveOptions created successfully with SaveFormat.Csv");
                
                // Salva la cartella di lavoro con le opzioni configurate
                workbook.Save("TxtSaveOptionsDemo.csv", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing TxtSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


