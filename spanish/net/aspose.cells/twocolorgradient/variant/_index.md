---
title: "TwoColorGradient.Variant"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TwoColorGradient. Gets and sets la variante del degradado"
type: docs
url: /es/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

Obtiene y establece la variante del degradado.

```csharp
public int Variant { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree un degradado bicolor con variante inicial
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // Cree y aplique el estilo a la celda A1
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // Muestre el valor actual de la variante
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // Modifique el valor de la variante
            gradient.Variant = 2;

            // Cree y aplique el estilo modificado a la celda B1
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // Haga las celdas más altas para visualizar los degradados
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


