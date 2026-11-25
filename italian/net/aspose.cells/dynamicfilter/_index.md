---
title: "Classe DynamicFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DynamicFilter. Rappresenta il filtro dinamico"
type: docs
url: /it/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Rappresenta il filtro dinamico.

```csharp
public class DynamicFilter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Ottiene e imposta il tipo di questo filtro dinamico. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Ottiene e imposta il valore massimo del filtro dinamico. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Ottiene e imposta il valore del filtro dinamico. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una cartella di lavoro e un foglio di lavoro (opzionale per il contesto)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Popola alcuni dati numerici di esempio
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Definisci un intervallo di autofiltro
                worksheet.AutoFilter.Range = "A1:A6";

                // Applica un filtro dinamico (AboveAverage) alla prima colonna
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // Recupera l'istanza DynamicFilter creata dall'AutoFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Imposta proprietà aggiuntive se desideri
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Visualizza le proprietà impostate
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Aggiorna il filtro per applicare le modifiche
                worksheet.AutoFilter.Refresh();

                // Salva la cartella di lavoro (i dati filtrati verranno salvati)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


