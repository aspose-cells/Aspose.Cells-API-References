---
title: "Format3D.SurfaceMaterialType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Format3D. Obtiene y establece el tipo de material que se combina con las propiedades de iluminación para dar el aspecto final de una forma. El valor predeterminado es PresetMaterialType.WarmMatte"
type: docs
url: /es/net/aspose.cells.drawing/format3d/surfacematerialtype/
---
## Format3D.SurfaceMaterialType property

Obtiene y establece el tipo de material que se combina con las propiedades de iluminación para dar el aspecto y la sensación final de una forma. El valor predeterminado es PresetMaterialType.WarmMatte.

```csharp
public PresetMaterialType SurfaceMaterialType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DPropertySurfaceMaterialTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);

            // Crear gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Configurar propiedades del formato 3D
            Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;
            format3D.LightingAngle = 30;
            format3D.SurfaceLightingType = LightRigType.BrightRoom;

            workbook.Save("Format3DPropertySurfaceMaterialTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with 3D chart using Metal surface material.");
        }
    }
}
```

### Ver también

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


