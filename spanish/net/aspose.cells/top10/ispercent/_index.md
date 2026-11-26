---
title: "Top10.IsPercent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Top10. Obtiene o establece si una regla superior/inferior n es una regla superior/inferior n por ciento. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

Obtener o establecer si una regla "top/bottom n" es una regla "top/bottom n percent". El valor predeterminado es false.

```csharp
public bool IsPercent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Agregar una regla de formato condicional Top10
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // Obtener la condición de formato Top10
            FormatCondition fc = fcc[0];
            
            // Establecer propiedades de Top10
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // Aplicar estilo de formato
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Guarda el libro de trabajo
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


