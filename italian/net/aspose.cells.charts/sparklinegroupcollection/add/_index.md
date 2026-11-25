---
title: "SparklineGroupCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SparklineGroupCollection. Aggiunge uno SparklineGroup con uno Sparkline alla collezione."
type: docs
url: /it/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Aggiunge un [`SparklineGroup`](../../sparklinegroup/) con un [`Sparkline`](../../sparkline/) alla collezione.

```csharp
public int Add(SparklineType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | SparklineType | Specifica il tipo del gruppo Sparkline. |

### Valore di ritorno

[`SparklineGroup`](../../sparklinegroup/) object index.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodAddWithSparklineTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per le sparklines
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // Ottieni la collezione del gruppo sparkline.
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // Chiama il metodo Add con il parametro SparklineType.
                int index = sparklineGroups.Add(SparklineType.Line);

                // Configura il gruppo sparkline.
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Aggiunge un [`SparklineGroup`](../../sparklinegroup/) con alcuni [`Sparkline`](../../sparkline/) alla collezione.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | SparklineType | Specifica il tipo del gruppo Sparkline. |
| dataRange | String | Specifica l'intervallo di dati del gruppo sparkline. |
| isVertical | Booleano | Specifica se tracciare gli sparklines dall'intervallo di dati per riga o per colonna. |
| locationRange | CellArea | Specifica dove posizionare le sparklines. |

### Valore di ritorno

[`SparklineGroup`](../../sparklinegroup/) object index.

### Osservazioni

Questo metodo creerà anche gli sparklines. Se *isVertical* è true, il numero di righe in dataRange e locationRange deve essere lo stesso. Se *isVertical* è false, il numero di colonne in dataRange e locationRange deve essere lo stesso.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionMethodAddWithSparklineTypeStringBooleanCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per le sparklines
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // Aggiungi il gruppo sparkline con i parametri specificati.
            sheet.SparklineGroups.Add(
                SparklineType.Line, 
                "A1:C1", 
                false, 
                CellArea.CreateCellArea("D1", "D1")
            );
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


