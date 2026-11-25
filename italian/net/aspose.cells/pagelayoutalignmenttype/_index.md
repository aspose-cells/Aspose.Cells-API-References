---
title: "Enum PageLayoutAlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.PageLayoutAlignmentType enum. Elenca i tipi di allineamento del layout di pagina"
type: docs
url: /it/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

Enumera i tipi di allineamento del layout di pagina.

```csharp
public enum PageLayoutAlignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Bottom | `0` | Rappresenta l'allineamento del layout di pagina inferiore. |
| Center | `1` | Rappresenta l'allineamento del layout di pagina centrale. |
| Left | `2` | Rappresenta l'allineamento del layout di pagina sinistro. |
| Right | `3` | Rappresenta l'allineamento del layout di pagina destro. |
| Top | `4` | Rappresenta l'allineamento del layout di pagina superiore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo di dati per il grafico
            chart.SetChartDataRange("A1:A4", true);

            // Imposta il titolo del grafico
            chart.Title.Text = "Sample Chart";

            // Salva la cartella di lavoro in un file
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // Esporta il grafico in PDF con un allineamento specifico del layout di pagina
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


