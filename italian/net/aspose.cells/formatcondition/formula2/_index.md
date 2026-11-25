---
title: "FormatCondition.Formula2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottiene e imposta il valore o l'espressione associata alla formattazione condizionale"
type: docs
url: /it/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale.

```csharp
public string Formula2 { get; set; }
```

### Osservazioni

Si prega di aggiungere tutte le aree prima di impostare la formula. Per impostare la formula per questa condizione, se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, booleano). Per un valore di testo che inizia con '=', l'utente può inserirlo come formula nel formato: \"=\\\"=...\\\"\"

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi formattazione condizionale
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // Definisci l'intervallo di celle
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // Aggiungi una condizione di formattazione con Formula2
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // Ottieni la condizione di formattazione
            FormatCondition formatCondition = formatConditions[0];

            // Restituisci le formule
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // Salva la cartella di lavoro
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


