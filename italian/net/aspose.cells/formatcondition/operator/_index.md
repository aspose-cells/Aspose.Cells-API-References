---
title: "FormatCondition.Operator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatCondition. Ottiene e imposta il tipo di operatore della formattazione condizionale"
type: docs
url: /it/net/aspose.cells/formatcondition/operator/
---
## FormatCondition.Operator property

Ottiene e imposta il tipo di operatore della formattazione condizionale.

```csharp
public OperatorType Operator { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyOperatorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Crea intervallo di celle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            
            // Aggiungi condizione
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "25");
            FormatCondition fc = fcc[conditionIndex];
            
            // Imposta lo stile
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;
            
            // Dimostra l'uso della proprietà Operator
            Console.WriteLine("Operator Type: " + fc.Operator);
            if (fc.Operator == OperatorType.Between)
            {
                Console.WriteLine("Condition is set to BETWEEN values");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


