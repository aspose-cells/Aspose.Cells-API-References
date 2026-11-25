---
title: "DynamicFilter.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DynamicFilter. Restituisce e imposta il valore del filtro dinamico"
type: docs
url: /it/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

Ottiene e imposta il valore del filtro dinamico.

```csharp
public object Value { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // Crea filtro automatico
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Visualizza il valore corrente del filtro
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // Modifica il valore del filtro per mostrare le date di aprile
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // Applica il filtro
            worksheet.AutoFilter.Refresh();

            // Salva il risultato
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


