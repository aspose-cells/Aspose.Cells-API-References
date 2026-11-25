---
title: "Cell.GetFormatConditions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Cell metodo. Ottiene le condizioni di formattazione che si applicano a questa cella"
type: docs
url: /it/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Ottiene le condizioni di formattazione che si applicano a questa cella.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Valore di ritorno

Restituisce l'oggetto [`FormatConditionCollection`](../../formatconditioncollection/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la raccolta di celle
            Cells cells = worksheet.Cells;
            
            // Aggiungi dati di esempio
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // Aggiungi condizione di formattazione alla cella A1
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // Ottieni le condizioni di formattazione per la cella A1
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // Restituisci il numero di condizioni di formattazione
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


