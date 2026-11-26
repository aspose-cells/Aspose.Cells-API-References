---
title: "FormatCondition.Priority"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. La prioridad de esta regla de formato condicional. Este valor se usa para determinar qué formato debe evaluarse y renderizarse. Los valores numéricos más bajos tienen mayor prioridad que los valores más altos, donde 1 es la prioridad más alta"
type: docs
url: /es/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

La prioridad de esta regla de formato condicional. Este valor se utiliza para determinar qué formato debe evaluarse y renderizarse. Los valores numéricos más bajos tienen mayor prioridad que los valores numéricos más altos, donde '1' es la prioridad más alta.

```csharp
public int Priority { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Agregar formato condicional
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // Agregar condiciones
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // Establecer prioridades
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // Demostrar el uso de la propiedad Priority
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // Guarda el libro de trabajo
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


