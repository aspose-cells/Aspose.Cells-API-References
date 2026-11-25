---
title: "FilterColumnCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumnCollection. Ottiene l'oggetto FilterColumn al campo speciale"
type: docs
url: /it/net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Ottiene l'oggetto [`FilterColumn`](../../filtercolumn/) al campo speciale.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| fieldIndex | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |

### Valore di ritorno

Restituisce l'oggetto [`FilterColumn`](../../filtercolumn/).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["A5"].PutValue("Date");

            // Applica filtro automatico
            sheet.AutoFilter.Range = "A1:A5";
            sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");

            // Accedi al filtro usando la proprietà Item
            AutoFilter filter = sheet.AutoFilter;
            FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
            CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
            CustomFilter firstFilter = customFilters[0];

            // Visualizza le proprietà del filtro
            Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
            Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);

            // Modifica il filtro
            firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);

            // Salva la cartella di lavoro
            wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


