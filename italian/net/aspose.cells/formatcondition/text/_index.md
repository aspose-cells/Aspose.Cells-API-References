---
title: "FormatCondition.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Il valore di testo in una regola di formattazione condizionale che contiene testo. Valido solo per i tipi containsText, notContainsText, beginsWith e endsWith. Il valore predefinito è null"
type: docs
url: /it/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

Il valore di testo in una regola di formattazione condizionale "text contains". Valida solo per type = containsText, notContainsText, beginsWith e endsWith. Il valore predefinito è null.

```csharp
public string Text { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi formattazione condizionale
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // Aggiungi condizione di testo
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // Imposta la proprietà text (dimostrando testo russo)
            formatCondition.Text = "вс";

            // Applica lo stile di formattazione
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // Applica alla cella A1
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // Salva e verifica
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


