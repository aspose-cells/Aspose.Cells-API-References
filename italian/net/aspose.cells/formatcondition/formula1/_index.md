---
title: "FormatCondition.Formula1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottiene e imposta il valore o l'espressione associata alla formattazione condizionale"
type: docs
url: /it/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Ottiene e imposta il valore o l'espressione associati alla formattazione condizionale.

```csharp
public string Formula1 { get; set; }
```

### Osservazioni

Si prega di aggiungere tutte le aree prima di impostare la formula. Per impostare la formula per questa condizione, se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, booleano). Per un valore di testo che inizia con '=', l'utente può inserirlo come formula nel formato: \"=\\\"=...\\\"\"

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["E1"].PutValue(50);
            
            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Imposta l'intervallo e il tipo di condizione
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // Accedi e visualizza la proprietà Formula1
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


