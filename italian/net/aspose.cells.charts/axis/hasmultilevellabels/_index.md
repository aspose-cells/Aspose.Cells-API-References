---
title: "Axis.HasMultiLevelLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà dell'asse. Indica se le etichette devono essere visualizzate a più livelli"
type: docs
url: /it/net/aspose.cells.charts/axis/hasmultilevellabels/
---
## Axis.HasMultiLevelLabels property

Indica se le etichette devono essere visualizzate a più livelli.

```csharp
public bool HasMultiLevelLabels { get; set; }
```

### Osservazioni

Valido solo per l'asse delle categorie.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyHasMultiLevelLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio con categorie a più livelli
            worksheet.Cells["A1"].PutValue("Main Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sub Category");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Value");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(8);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dei dati del grafico includendo categorie a più livelli
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "A1:B3";
            
            // Verifica e visualizza la proprietà HasMultiLevelLabels
            Console.WriteLine("HasMultiLevelLabels: " + chart.CategoryAxis.HasMultiLevelLabels);
            
            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyHasMultiLevelLabelsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


