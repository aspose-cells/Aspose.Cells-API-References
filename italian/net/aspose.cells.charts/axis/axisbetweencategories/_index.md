---
title: "Axis.AxisBetweenCategories"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta se l'asse dei valori attraversa l'asse delle categorie tra le categorie"
type: docs
url: /it/net/aspose.cells.charts/axis/axisbetweencategories/
---
## Axis.AxisBetweenCategories property

Rappresenta se l'asse dei valori attraversa l'asse delle categorie tra le categorie.

```csharp
public bool AxisBetweenCategories { get; set; }
```

### Osservazioni

Questa proprietà si applica solo agli assi delle categorie e non si applica ai grafici 3-D.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisBetweenCategoriesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Categories");
            worksheet.Cells["B1"].PutValue("Values");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Category {i}");
                worksheet.Cells[$"B{i+1}"].PutValue(i * 10);
            }

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta i dati del grafico
            chart.NSeries.Add("B2:B6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Configura l'asse delle categorie
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.AxisBetweenCategories = false; // Core property demonstration
            categoryAxis.TickLabels.RotationAngle = 45;

            // Salva la cartella di lavoro
            workbook.Save("AxisBetweenCategoriesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


