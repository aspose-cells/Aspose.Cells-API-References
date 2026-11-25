---
title: "DataLabels.SeparatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Ottiene o imposta il tipo di separatore usato per le etichette dati su un grafico"
type: docs
url: /it/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Ottiene o imposta il tipo di separatore utilizzato per le etichette dati in un grafico.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Osservazioni

Per impostare un separatore personalizzato, impostare la proprietà `SeparatorType` su Custom e quindi specificare il valore atteso per [`SeparatorValue`](../separatorvalue/).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita le etichette dei dati
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // Imposta il tipo di separatore
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


