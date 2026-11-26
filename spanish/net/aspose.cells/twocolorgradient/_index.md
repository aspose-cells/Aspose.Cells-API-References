---
title: "Clase TwoColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.TwoColorGradient. Representa un degradado de dos colores"
type: docs
url: /es/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

Representa un degradado de dos colores.

```csharp
public class TwoColorGradient
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | Obtiene y establece el primer color del degradado. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | Obtiene y establece el segundo color del degradado. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Obtiene y establece el estilo de sombreado del degradado. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Obtiene y establece la variante del degradado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inicializar TwoColorGradient con parámetros del constructor
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // Modificar las propiedades del degradado después de la inicialización
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // Crear estilo de celda y aplicar degradado
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // Aplicar estilo a la celda y agregar contenido
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // Ajustar las dimensiones de la celda para que sea visible
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // Guardar el resultado con formato de degradado
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


