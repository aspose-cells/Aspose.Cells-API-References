---
title: "ConditionalFormattingCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingCollection. Obtiene el elemento FormatConditions en el índice especificado"
type: docs
url: /es/net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Obtiene el elemento FormatConditions en el índice especificado.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Agregar formato condicional
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            // Agregar condición de formato
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "50");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Acceder y demostrar el uso de la propiedad Item
            FormatConditionCollection firstFormatting = sheet.ConditionalFormattings[0];
            Console.WriteLine($"First formatting has {firstFormatting.Count} conditions");
            Console.WriteLine($"First condition operator: {firstFormatting[0].Operator}");
        }
    }
}
```

### Ver también

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


