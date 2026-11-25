---
title: "FormatCondition.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottiene e imposta se il tipo di formattazione condizionale"
type: docs
url: /it/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Ottiene e imposta se il tipo di formattazione condizionale.

```csharp
public FormatConditionType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Crea formattazione condizionale
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Aggiungi una condizione di formattazione con tipo espressione (parametri corretti)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // Imposta lo stile per la condizione
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // Salva la cartella di lavoro
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


