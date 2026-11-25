---
title: "ChartCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartCollection. Ottiene l'elemento Chart all'indice specificato"
type: docs
url: /it/net/aspose.cells.charts/chartcollection/item/
---
## ChartCollection indexer (1 of 2)

Ottiene l'elemento [`Chart`](../../chart/) all'indice specificato.

```csharp
public Chart this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            
            // Accedi al grafico usando la proprietà Item
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico e il titolo
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Title.Text = "Sample Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Chart created successfully with Item property access.");
        }
    }
}
```

### Vedi anche

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ChartCollection indexer (2 of 2)

Ottiene il grafico per nome.

```csharp
public Chart this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome del grafico. |

### Valore di ritorno

Il grafico.

### Osservazioni

Il nome predefinito del grafico è null. Quindi devi impostare esplicitamente il nome del grafico.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Aggiungi un grafico al foglio di lavoro
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);

                // Accedi al grafico usando la proprietà Item (indicizzatore)
                Chart chart = worksheet.Charts[chartIndex];

                // Visualizza le informazioni sul grafico
                Console.WriteLine("Chart type: " + chart.Type);
                Console.WriteLine("Chart name: " + chart.Name);

                // Salva la cartella di lavoro
                workbook.Save("ChartCollectionItemDemo.xlsx");

                Console.WriteLine("Chart created and accessed successfully using Item property.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


