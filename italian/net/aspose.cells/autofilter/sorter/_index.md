---
title: "AutoFilter.Sorter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFilter. Ottiene l'ordinatore dei dati"
type: docs
url: /it/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Ottiene l'ordinatore dei dati.

```csharp
public DataSorter Sorter { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Crea intervallo di filtro automatico
            worksheet.AutoFilter.Range = "A1:B4";

            // Ottieni il filtro automatico
            AutoFilter filter = worksheet.AutoFilter;

            // Applica filtro
            filter.Filter(1, "10");

            // Ordina usando la proprietà Sorter
            filter.Sorter.Sort();

            // Salva la cartella di lavoro
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


