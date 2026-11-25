---
title: "Enum DataBarNegativeColorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DataBarNegativeColorType enum. Specifica se utilizzare lo stesso colore del bordo e di riempimento delle barre dati positive"
type: docs
url: /it/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

Specifica se utilizzare lo stesso colore di bordo e di riempimento delle barre dei dati positive.

```csharp
public enum DataBarNegativeColorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Color | `0` | Usa il colore specificato nella finestra di dialogo Valore negativo e impostazioni dell'asse o utilizzando le proprietà ColorType e BorderColorType dell'oggetto NegativeBarFormat. |
| SameAsPositive | `1` | Usa lo stesso colore delle barre dati positive. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Imposta le proprietà della barra dati
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Imposta le proprietà del formato della barra negativa
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Salva la cartella di lavoro
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


