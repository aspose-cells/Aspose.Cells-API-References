---
title: "LoadFilter.LoadFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadFilter-Konstruktor. Erstellt ein LoadFilter mit den Standardfilteroptionen LoadDataFilterOptions.All"
type: docs
url: /de/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Erstellt einen LoadFilter mit den Standardfilteroptionen LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues LoadFilter mit dem Standardkonstruktor
            LoadFilter filter = new LoadFilter();
            
            // Erstelle Ladeoptionen und weise den Filter zu
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // Lade Arbeitsmappe mit dem Filter
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // Demonstriere die Verwendung, indem du Arbeitsblätter zählst
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // Zeige gefilterte Zellendaten (alle Zellen werden standardmäßig geladen)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### Siehe auch

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Erstellt einen LoadFilter mit den angegebenen Filteroptionen.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | LoadDataFilterOptions | die Standardfilteroptionen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bereite Daten für die Methodenparameter vor (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // Rufe die #ctor-Methode mit den spezifischen Parametertypen auf
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Verarbeite oder zeige das Ergebnis an
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Zeige die Wirkung des Methodenaufrufs
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


