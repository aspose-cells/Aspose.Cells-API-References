---
title: "LoadFilter.LoadFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadFilter-konstruktor. Skapar en LoadFilter med standardfilteralternativ LoadDataFilterOptions.All"
type: docs
url: /sv/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Skapar ett LoadFilter med standardfilteralternativ LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny LoadFilter med standardkonstruktor
            LoadFilter filter = new LoadFilter();
            
            // Skapa laddningsalternativ och tilldela filtret
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // Läs in arbetsbok med filtret
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // Demonstrera användning genom att räkna kalkylblad
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // Visa filtrerad celldata (alla celler laddas som standard)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### Se även

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Skapar ett LoadFilter med angivna filteralternativ.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | LoadDataFilterOptions | standardfilteralternativen |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered data för metodparametrarna (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // Anropa #ctor-metoden med de specifika parametertyperna
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Bearbeta eller visa resultatet
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Visa effekten av metodanropet
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


