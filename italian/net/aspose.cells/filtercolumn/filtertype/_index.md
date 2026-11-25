---
title: "FilterColumn.FilterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene e imposta il tipo di dati di filtraggio"
type: docs
url: /it/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Ottiene e imposta il tipo di filtraggio dei dati.

```csharp
public FilterType FilterType { get; set; }
```

### Osservazioni

L'oggetto filtro corrispondente verrà creato quando questa proprietà è impostata e la proprietà corrispondente dovrebbe essere usata per ottenere l'oggetto filtro di conseguenza:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // Applica filtro automatico usando un intervallo di stringhe
            sheet.AutoFilter.Range = "A1:B4";

            // Aggiungi diversi tipi di filtro per dimostrare la proprietà FilterType
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // Ottieni le colonne di filtro
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Visualizza FilterType per ogni colonna
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // Salva la cartella di lavoro
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


