---
title: "DynamicFilter.MaxValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DynamicFilter. Ottiene e imposta il valore massimo del filtro dinamico"
type: docs
url: /it/net/aspose.cells/dynamicfilter/maxvalue/
---
## DynamicFilter.MaxValue property

Ottiene e imposta il valore massimo del filtro dinamico.

```csharp
public object MaxValue { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati numerici di esempio
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);

            // Crea filtro automatico
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Applica filtro dinamico con criteri di intervallo
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Visualizza il MaxValue corrente
            Console.WriteLine("Current MaxValue: " + filter.MaxValue);

            // Poiché DynamicFilterType.Between non esiste, utilizzeremo un approccio diverso
            // Ad esempio, possiamo usare un filtro personalizzato invece
            worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, 20);
            worksheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, 40);

            // Applica il filtro
            worksheet.AutoFilter.Refresh();

            // Salva il risultato
            workbook.Save("DynamicFilterMaxValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


