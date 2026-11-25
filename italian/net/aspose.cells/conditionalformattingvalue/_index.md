---
title: "Classe ConditionalFormattingValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ConditionalFormattingValue. Descrive i valori dei punti di interpolazione in una scala gradiente dataBar o iconSet"
type: docs
url: /it/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

Descrive i valori dei punti di interpolazione in una scala gradiente, dataBar o iconSet.

```csharp
public class ConditionalFormattingValue
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Ottieni o imposta il flag Maggiore o Uguale. Usa solo per set di icone, determina se questo valore soglia utilizza l'operatore maggiore o uguale. 'false' indica che viene usato 'maggiore' invece di 'maggiore o uguale'. Il valore predefinito è true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Ottieni o imposta il tipo di questo oggetto di valore di formattazione condizionale. Impostare il tipo su FormatConditionValueType.Min o FormatConditionValueType.Max imposterà automaticamente "Value" a null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Ottieni o imposta il valore di questo oggetto di valore di formattazione condizionale. Deve essere usato in combinazione con Type. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Aggiunge condizione
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Impostazione delle proprietà per ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Impostazione valore minimo
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Impostazione valore medio
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Impostazione valore massimo
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Salva la cartella di lavoro
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


