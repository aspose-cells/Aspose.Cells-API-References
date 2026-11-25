---
title: "ConditionalFormattingValue.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingValue. Ottieni o imposta il valore di questo oggetto di valore di formattazione condizionale. Deve essere usata in congiunzione con Type"
type: docs
url: /it/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Ottieni o imposta il valore di questo oggetto di valore di formattazione condizionale. Deve essere usato in combinazione con Type.

```csharp
public object Value { get; set; }
```

### Osservazioni

Se il valore è una stringa e inizia con "=", verrà elaborato come una formula, altrimenti lo elaboreremo come un valore semplice.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
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
            worksheet.Cells["A4"].PutValue(40);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Crea formattazione condizionale per il set di icone
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // Ottieni gli oggetti di valore di formattazione condizionale
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // Imposta i valori per le icone
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // Dimostra l'uso della proprietà Value
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


