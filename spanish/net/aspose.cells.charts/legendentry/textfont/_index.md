---
title: "LegendEntry.TextFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LegendEntry. Obtiene un objeto Font del objeto LegendEntry especificado"
type: docs
url: /es/net/aspose.cells.charts/legendentry/textfont/
---
## LegendEntry.TextFont property

Obtiene un objeto [`Font`](../font/) del objeto LegendEntry especificado.

```csharp
[Obsolete("Use LegendEntry.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad LegendEntry.Font. Esta propiedad será eliminada 12 meses después a partir de ENERO de 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyTextFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(45);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Habilitar leyenda
            chart.ShowLegend = true;
            Legend legend = chart.Legend;

            // Acceder a la primera entrada de leyenda y modificar sus propiedades TextFont
            LegendEntry legendEntry = legend.LegendEntries[0];
            Aspose.Cells.Font font = legendEntry.TextFont;
            
            // Establecer varias propiedades de fuente
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Guarda el libro de trabajo
            workbook.Save("LegendEntryTextFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


