---
title: "Classe DataBarBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataBarBorder. Rappresenta il bordo delle barre dei dati specificato da una regola di formattazione condizionale"
type: docs
url: /it/net/aspose.cells/databarborder/
---
## DataBarBorder class

Rappresenta il bordo delle barre dati specificate da una regola di formattazione condizionale.

```csharp
public class DataBarBorder
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Ottiene o imposta il colore del bordo delle barre dei dati specificato da una regola di formattazione condizionale. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Ottiene o imposta il tipo del bordo delle barre dei dati specificato da una regola di formattazione condizionale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // Creazione di una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            // Accesso al primo foglio di lavoro nella cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // Aggiunta di una formattazione condizionale vuota
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Definizione di un'area di celle per la formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Aggiunta di una condizione di tipo DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // Accesso al DataBar
            DataBar dataBar = formatCondition.DataBar;

            // Impostazione delle proprietà del DataBar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // Accesso e impostazione delle proprietà del DataBarBorder
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // Salvataggio del file Excel
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


