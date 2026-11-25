---
title: "FormatConditionCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatConditionCollection. Ottiene la condizione di formattazione per indice"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Ottiene la condizione di formattazione per indice.

```csharp
public FormatCondition this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | l'indice della condizione di formattazione da restituire. |

### Valore di ritorno

la condizione di formattazione

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi una raccolta di condizioni di formattazione
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Aggiungi una condizione di formattazione
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // Accedi alla prima condizione di formattazione usando la proprietà Item
            FormatCondition condition = fcc[0];
            
            // Visualizza le formule
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // Modifica le formule usando la proprietà Item
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // Visualizza le formule modificate
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


