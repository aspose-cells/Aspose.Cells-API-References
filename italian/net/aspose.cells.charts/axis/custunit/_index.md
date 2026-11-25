---
title: "Axis.CustUnit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Specifica un valore personalizzato per l'unità di visualizzazione"
type: docs
url: /it/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

Specifica un valore personalizzato per l'unità di visualizzazione.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà Axis.CustomUnit. Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Aggiungi un grafico e imposta il suo intervallo di dati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Ottieni l'asse dei valori
            Axis valueAxis = chart.ValueAxis;

            // Visualizza il valore corrente di CustUnit (proprietà obsoleta)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // Imposta un nuovo valore di unità personalizzata (1,000,000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // Visualizza il nuovo valore di CustUnit
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // Salva il risultato
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


