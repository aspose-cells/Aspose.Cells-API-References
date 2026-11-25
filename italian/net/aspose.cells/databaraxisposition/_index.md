---
title: "Enum DataBarAxisPosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.DataBarAxisPosition. Specifica la posizione dell'asse per un intervallo di celle con formattazione condizionale come barre dei dati"
type: docs
url: /it/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

Specifica la posizione dell'asse per un intervallo di celle con formattazione condizionale come barre dei dati.

```csharp
public enum DataBarAxisPosition
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Visualizza l'asse in una posizione variabile basata sul rapporto tra il valore negativo minimo e il valore positivo massimo nell'intervallo. I valori positivi sono visualizzati in direzione da sinistra a destra. I valori negativi sono visualizzati in direzione da destra a sinistra. Quando tutti i valori sono positivi o tutti i valori sono negativi, non viene visualizzato alcun asse. |
| Midpoint | `1` | Visualizza l'asse al punto medio della cella indipendentemente dal set di valori nell'intervallo. I valori positivi sono visualizzati in direzione da sinistra a destra. I valori negativi sono visualizzati in direzione da destra a sinistra. |
| None | `2` | Nessun asse viene visualizzato e sia i valori positivi che quelli negativi sono visualizzati in direzione da sinistra a destra. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarAxisPositionDemo
    {
        public static void DataBarAxisPositionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Accesso al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiunta di una regola di formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Impostazione dell'intervallo di formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Aggiunta di una condizione di barra dei dati
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Impostazione delle proprietà per la barra dei dati
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // Inserimento dei valori delle celle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // Salvataggio del file Excel
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


