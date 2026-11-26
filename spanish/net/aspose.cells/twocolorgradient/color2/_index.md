---
title: "TwoColorGradient.Color2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TwoColorGradient. Obtiene y establece el segundo color del degradado"
type: docs
url: /es/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

Obtiene y establece el segundo color del degradado.

```csharp
public Color Color2 { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de degradado de dos colores
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // Crear el primer estilo con el degradado inicial
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // Mostrar el valor actual de Color2
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // Modificar la propiedad Color2
            gradient.Color2 = Color.Red;

            // Crear el segundo estilo con el degradado modificado
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // Ajustar filas para la visibilidad
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // Guarda el libro de trabajo
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### Ver también

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


