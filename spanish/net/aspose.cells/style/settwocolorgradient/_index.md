---
title: "Style.SetTwoColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Establece el relleno especificado a un degradado de dos colores"
type: docs
url: /es/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Establece el relleno especificado a un degradado bicolor.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color1 | Color | Un color de degradado. |
| color2 | Color | Dos colores de degradado. |
| gradientStyleType | GradientStyleType | Estilo de sombreado de degradado. |
| variant | Int32 | La variante del degradado. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree un objeto de estilo
            Style style = workbook.CreateStyle();

            // Establece un degradado de dos colores para el estilo
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // Verifica la configuración del degradado
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // Guarda el libro de trabajo
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


