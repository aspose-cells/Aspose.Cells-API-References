---
title: "ConditionalFormattingIcon.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingIcon. Ottiene e imposta il tipo del set di icone"
type: docs
url: /it/net/aspose.cells/conditionalformattingicon/type/
---
## ConditionalFormattingIcon.Type property

Ottiene e imposta il tipo di set di icone.

```csharp
public IconSetType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyTypeDemo
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

            // Aggiungi formattazione condizionale con set di icone
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fc = cfs[index];
            fc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            int conditionIndex = fc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fc[conditionIndex];
            condition.IconSet.Type = IconSetType.Symbols3;
            
            // Applica la formattazione e calcola
            workbook.CalculateFormula();

            // Ottieni il risultato della formattazione e dimostra la proprietà Type
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("Icon Set Type: " + formattingResult.ConditionalFormattingIcon.Type);
            Console.WriteLine("Icon Index: " + formattingResult.ConditionalFormattingIcon.Index);
        }
    }
}
```

### Vedi anche

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


