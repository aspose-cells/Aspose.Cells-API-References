---
title: "ConditionalFormattingIconCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingIconCollection. Obtiene el elemento ConditionalFormattingIcon en el índice especificado."
type: docs
url: /es/net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

Obtiene el elemento ConditionalFormattingIcon en el índice especificado.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;
            int index = cformattings.Add();
            FormatConditionCollection fcs = cformattings[index];

            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 });
            fcs.AddArea(new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 });

            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];
            cond.IconSet.Type = IconSetType.ArrowsGray3;

            // Demostrar el uso de la propiedad Item
            ConditionalFormattingIcon icon = cond.IconSet.CfIcons[0];
            icon.Type = IconSetType.Arrows3;
            icon.Index = 0;

            workbook.Save("ConditionalFormattingIconCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


