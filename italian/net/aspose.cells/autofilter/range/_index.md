---
title: "AutoFilter.Range"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFilter. Rappresenta l'intervallo a cui si applica l'AutoFilter specificato"
type: docs
url: /it/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Rappresenta l'intervallo a cui si applica l'AutoFilter specificato.

```csharp
public string Range { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // Applica il filtro automatico all'intervallo A1:A5
            sheet.AutoFilter.Range = "A1:A5";

            // Visualizza l'intervallo del filtro automatico
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // Salva la cartella di lavoro
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


