---
title: "Classe FilterColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FilterColumn. Rappresenta un filtro per una singola colonna o una colonna nella tabella"
type: docs
url: /it/net/aspose.cells/filtercolumn/
---
## FilterColumn class

Rappresenta un filtro per una singola colonna o per una colonna nella tabella.

```csharp
public class FilterColumn
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | Ottiene [`ColorFilter`](../colorfilter/) per filtrare i dati per colore. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | Ottiene [`CustomFilterCollection`](../customfiltercollection/) per filtrare i dati per criteri personalizzati. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | Ottiene [`DynamicFilter`](./dynamicfilter/) per filtrare con criteri dinamici. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Ottiene e imposta lo spostamento della colonna nell'intervallo. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsolete.**) Ottiene e imposta la condizione del filtraggio dei dati. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Ottiene e imposta il tipo di filtraggio dei dati. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | Ottiene [`FilterValueCollection`](../filtervaluecollection/) per filtrare i dati per etichette o data/ora. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | Ottiene [`IconFilter`](./iconfilter/) per filtrare i dati per icona. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Obsolete.**) Ottiene [`MultipleFilterCollection`](../multiplefiltercollection/) per filtrare i dati per etichette o data/ora. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | Ottiene [`Top10Filter`](./top10filter/) per filtrare i dati per classifica. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | Seleziona tutto. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;

namespace AsposeCellsExamples
{
    public class FilterColumnDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // Applica AutoFilter all'intervallo
            sheet.AutoFilter.SetRange(0, 0, 3);

            // Aggiungi un filtro alla prima colonna (Nome)
            sheet.AutoFilter.AddFilter(0, "John");

            // Aggiungi un filtro alla seconda colonna (Età)
            sheet.AutoFilter.AddFilter(1, "30");

            // Aggiorna il filtro per applicarlo
            sheet.AutoFilter.Refresh();

            // Accedi a FilterColumnCollection
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Accedi al primo FilterColumn
            FilterColumn filterColumn = filterColumns[0];

            // Visualizza le proprietà di FilterColumn
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // Salva la cartella di lavoro
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


