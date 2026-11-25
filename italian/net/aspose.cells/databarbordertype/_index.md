---
title: "Enum DataBarBorderType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DataBarBorderType enum. Specifica il tipo di bordo di una barra dati"
type: docs
url: /it/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

Specifica il tipo di bordo di una barra dei dati.

```csharp
public enum DataBarBorderType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | La barra dati non ha bordi. |
| Solid | `1` | La barra dati ha un bordo solido. |

### Esempi

```csharp
using Aspose.Cells;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderTypeDemo
    {
        public static void DataBarBorderTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Aggiungi la formattazione condizionale al foglio di lavoro
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Definisci un'area di celle per la formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Aggiungi una regola di formattazione condizionale a barra dati
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // Accedi all'oggetto DataBar
            DataBar dataBar = fc.DataBar;

            // Imposta il colore della barra dati
            dataBar.Color = Color.Blue;

            // Imposta la lunghezza minima e massima della barra dati
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Imposta il tipo di bordo della barra dati
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Imposta il colore del bordo della barra dati
            dataBar.BarBorder.Color = Color.Red;

            // Salva la cartella di lavoro
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


