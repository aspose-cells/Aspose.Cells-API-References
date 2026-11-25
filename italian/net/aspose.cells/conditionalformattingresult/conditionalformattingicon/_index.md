---
title: "ConditionalFormattingResult.ConditionalFormattingIcon"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConditionalFormattingResult proprietà. Restituisce l'immagine del set di icone"
type: docs
url: /it/net/aspose.cells/conditionalformattingresult/conditionalformattingicon/
---
## ConditionalFormattingResult.ConditionalFormattingIcon property

Ottiene l'immagine del set di icone.

```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingIconDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e formattazione condizionale
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Aggiungi formattazione condizionale al set di icone
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Calcola le formule e ottieni il risultato della formattazione condizionale
            workbook.CalculateFormula();
            ConditionalFormattingResult result = worksheet.Cells["A1"].GetConditionalFormattingResult();

            // Dimostra la proprietà ConditionalFormattingIcon
            if (result != null && result.ConditionalFormattingIcon != null)
            {
                Console.WriteLine("Icon Type: " + result.ConditionalFormattingIcon.Type);
                Console.WriteLine("Icon Index: " + result.ConditionalFormattingIcon.Index);
            }
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


