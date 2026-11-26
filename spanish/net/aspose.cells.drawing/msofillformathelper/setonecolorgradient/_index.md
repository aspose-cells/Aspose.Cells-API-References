---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método MsoFillFormatHelper. Establece el relleno especificado a un degradado de un solo color"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Establece el relleno especificado a un degradado de un solo color.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | Color | Un color de degradado. |
| grado | Double | El grado del degradado. Puede ser un valor de 0.0 (oscuro) a 1.0 (claro). |
| estilo | GradientStyleType | Estilo de sombreado de degradado. |
| variant | Int32 | La variante del degradado. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Coloca una etiqueta simple en la hoja para dar contexto
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // Crea una instancia de MsoFillFormatHelper usando reflexión (sin constructor público)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Parámetros del degradado
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // Aplica el degradado de un solo color
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // Opcional: muestra que las propiedades pueden leerse después de la llamada
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // Guarda el libro de trabajo (no se verá ningún cambio visual porque el helper no está adjunto a una forma)
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


