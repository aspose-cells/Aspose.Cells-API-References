---
title: "LoadFilter.LoadFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore LoadFilter. Crea un LoadFilter con le opzioni di filtro predefinite LoadDataFilterOptions.All"
type: docs
url: /it/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Crea un LoadFilter con le opzioni di filtro predefinite LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo LoadFilter con il costruttore predefinito
            LoadFilter filter = new LoadFilter();
            
            // Crea le opzioni di caricamento e assegna il filtro
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // Carica la cartella di lavoro con il filtro
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // Dimostrare l'uso contando i fogli di lavoro
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // Mostra i dati delle celle filtrate (tutte le celle caricate per impostazione predefinita)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### Vedi anche

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Crea un LoadFilter con le opzioni di filtro specificate.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | LoadDataFilterOptions | le opzioni di filtro predefinite |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // Chiama il metodo #ctor con i tipi di parametro specifici
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Elabora o visualizza il risultato
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Mostra l'effetto della chiamata al metodo
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


