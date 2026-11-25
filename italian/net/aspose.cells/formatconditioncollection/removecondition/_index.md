---
title: "FormatConditionCollection.RemoveCondition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FormatConditionCollection. Rimuove la condizione di formattazione per indice"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

Rimuove la condizione di formattazione per indice.

```csharp
public void RemoveCondition(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice della condizione di formattazione da rimuovere. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la collezione delle condizioni di formattazione
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // Aggiungi alcune condizioni di esempio
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // Visualizza il conteggio iniziale
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // Rimuovi la prima condizione
                formatConditions.RemoveCondition(index1);
                
                // Visualizza il conteggio aggiornato
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // Salva la cartella di lavoro
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


