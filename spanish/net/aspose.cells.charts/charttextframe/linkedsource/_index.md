---
title: "ChartTextFrame.LinkedSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Obtiene y establece una referencia a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Obtiene y establece una referencia a la hoja de cálculo.

```csharp
public virtual string LinkedSource { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyLinkedSourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["P1"].PutValue("Chart Title");
            
            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer el título del gráfico y enlazarlo a la celda P1
            chart.Title.Text = "Linked Title";
            chart.Title.LinkedSource = "='" + worksheet.Name + "'!$P$1";
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar la fuente vinculada
            Console.WriteLine("Chart Title Linked Source: " + chart.Title.LinkedSource);
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


