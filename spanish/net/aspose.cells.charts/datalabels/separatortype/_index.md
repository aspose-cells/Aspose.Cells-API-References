---
title: "DataLabels.SeparatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Obtiene o establece el tipo de separador usado para las etiquetas de datos en un gráfico"
type: docs
url: /es/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Obtiene o establece el tipo de separador utilizado para las etiquetas de datos en un gráfico.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Observaciones

Para establecer un separador personalizado, establezca la propiedad `SeparatorType` como Custom y luego especifique el valor esperado para [`SeparatorValue`](../separatorvalue/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // Establecer tipo de separador
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


