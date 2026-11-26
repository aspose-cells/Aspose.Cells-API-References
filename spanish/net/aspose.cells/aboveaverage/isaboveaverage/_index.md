---
title: "AboveAverage.IsAboveAverage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AboveAverage. Obtenga o establezca la bandera que indica si la regla es una regla de por encima del promedio. true indica por encima del promedio. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Obtenga o establezca la bandera que indica si la regla es una regla "above average". 'true' indica "above average". El valor predeterminado es true.

```csharp
public bool IsAboveAverage { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();
            
            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para demostrar el formato condicional
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Agregar un formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establecer el rango del formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Agregar una condición AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Configurar las propiedades AboveAverage
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // Guardar el archivo Excel
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


