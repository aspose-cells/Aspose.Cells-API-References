---
title: "ChartFrame.BackgroundMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene y establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores."
type: docs
url: /es/net/aspose.cells.charts/chartframe/backgroundmode/
---
## ChartFrame.BackgroundMode property

Obtiene y establece el modo de visualización del fondo. Esta propiedad solo es válida en Excel 2003 o versiones anteriores.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode BackgroundMode { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad ChartFrame.Area.FillFormat.FillType. Por ejemplo, si necesita establecer BackgroundMode a Opaque, puede usar el siguiente código: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Esta propiedad será eliminada 12 meses después a partir de febrero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["B4"].PutValue(20);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Establecer datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar la propiedad BackgroundMode
            chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
            chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;

            // Guarda el libro de trabajo
            workbook.Save("ChartBackgroundModeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


