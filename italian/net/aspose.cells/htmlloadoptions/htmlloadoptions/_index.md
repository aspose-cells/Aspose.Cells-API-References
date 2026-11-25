---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore HtmlLoadOptions. Crea un'opzione per il caricamento del file"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Crea un'opzione per il caricamento del file.

```csharp
public HtmlLoadOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento HTML usando il costruttore
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // Carica il file HTML con le opzioni
            Workbook workbook = new Workbook("example.html", loadOptions);

            // Accedi ai dati dall'HTML caricato
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Crea un'opzione per il caricamento del file.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
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

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di HtmlLoadOptions usando il costruttore con il parametro LoadFormat
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // Imposta alcune proprietà di HtmlLoadOptions
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Crea una cartella di lavoro usando le opzioni di caricamento
                Workbook workbook = new Workbook("input.html", loadOptions);

                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];

                // Visualizza alcune informazioni sull'HTML caricato
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Salva la cartella di lavoro
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


