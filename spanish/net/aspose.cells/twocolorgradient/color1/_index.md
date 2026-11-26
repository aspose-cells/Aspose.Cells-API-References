---
title: "TwoColorGradient.Color1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TwoColorGradient. Obtiene y establece el primer color del degradado"
type: docs
url: /es/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

Obtiene y establece el primer color del degradado.

```csharp
public Color Color1 { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Crear estilo con relleno de degradado
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // Inicializar degradado de dos colores
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // Aplicar degradado al estilo de celda
            cell.SetStyle(style);
            
            // Leer el color inicial
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // Modificar el color del degradado y volver a aplicar
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // Verificar la actualización
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // Demostración visual en el archivo de salida
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### Ver también

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


