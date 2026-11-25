---
title: "ConditionalFormattingIcon.Index"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingIcon. Ottiene e imposta l'indice delle icone nel set di icone"
type: docs
url: /it/net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

Ottiene e imposta l'indice dell'icona nel set di icone.

```csharp
public int Index { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Aggiungi formattazione condizionale al set di icone
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.IconSet);
            
            // Imposta le proprietà del set di icone
            FormatCondition condition = fcc[0];
            condition.IconSet.Type = IconSetType.Arrows3;
            ConditionalFormattingIconCollection icons = condition.IconSet.CfIcons;

            // Visualizza l'indice di ogni icona
            Console.WriteLine("Icon Indexes:");
            for (int i = 0; i < icons.Count; i++)
            {
                Console.WriteLine($"Icon {i}: Index = {icons[i].Index}");
            }

            // Modifica e mostra la proprietà indice
            icons[1].Index = 2;
            Console.WriteLine($"Modified Icon 1 Index: {icons[1].Index}");
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


