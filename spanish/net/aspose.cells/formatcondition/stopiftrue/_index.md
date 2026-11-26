---
title: "FormatCondition.StopIfTrue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Verdadero, ninguna regla con menor prioridad puede aplicarse sobre esta regla cuando esta regla se evalúa como verdadera. Solo se aplica a Excel 2007"
type: docs
url: /es/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

True, ninguna regla con prioridad inferior puede aplicarse sobre esta regla, cuando esta regla se evalúa como verdadera. Solo se aplica a Excel 2007;

```csharp
public bool StopIfTrue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Agregar condición y establecer StopIfTrue
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // Agregar otra condición que normalmente sobrescribiría la primera
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // Guarda el libro de trabajo
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


