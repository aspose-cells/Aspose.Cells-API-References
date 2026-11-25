---
title: "ConditionalFormattingValue.IsGTE"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingValue. Ottieni o imposta il flag Maggiore O Uguale. Da usare solo per set di icone, determina se questo valore soglia utilizza l'operatore maggiore o uguale. false indica che viene usato maggiore invece di maggiore o uguale. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Ottieni o imposta il flag Maggiore o Uguale. Usa solo per set di icone, determina se questo valore soglia utilizza l'operatore maggiore o uguale. 'false' indica che viene usato 'maggiore' invece di 'maggiore o uguale'. Il valore predefinito è true.

```csharp
public bool IsGTE { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // Aggiungi formattazione condizionale
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // Crea un formato di scala di colori
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // Configura una scala a 2 colori
            fc.ColorScale.Is3ColorScale = false;
            
            // Imposta il formato del valore massimo (dimostrando IsGTE)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // Imposta il formato del valore minimo
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // Salva la cartella di lavoro
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


