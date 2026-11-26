---
title: "ChartFrame.Background"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene y establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores."
type: docs
url: /es/net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

Obtiene y establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad ChartFrame.Area.FillFormat.FillType. Por ejemplo, si necesita establecer BackgroundMode a Opaque, puede usar el siguiente código: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Esta propiedad será eliminada 12 meses después a partir de ENERO 2012. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Configurar datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurar etiquetas de datos con ajustes de fondo
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Background = BackgroundMode.Transparent;

            // Guarda el libro de trabajo
            workbook.Save("ChartBackgroundDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


