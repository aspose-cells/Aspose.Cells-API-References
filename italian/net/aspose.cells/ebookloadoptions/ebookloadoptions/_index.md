---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore EbookLoadOptions. Crea un'opzione per caricare il file ebook"
type: docs
url: /it/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

Crea un'opzione per caricare il file ebook.

```csharp
public EbookLoadOptions()
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un'istanza di EbookLoadOptions usando il costruttore
            EbookLoadOptions options = new EbookLoadOptions();

            // Imposta alcune proprietà di base
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Carica un file ebook con le opzioni specificate
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Salva come file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

Crea un'opzione di caricamento del file ebook.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
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

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di EbookLoadOptions con il parametro LoadFormat
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Mostra conferma
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Esempio di utilizzo: carica una cartella di lavoro con queste opzioni
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Salva il risultato
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


