---
title: "MsoFillFormatHelper.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFillFormatHelper. Indica si hay relleno"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Indica si hay relleno.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una etiqueta para que el ejemplo sea significativo
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // Crear una instancia de MsoFillFormatHelper usando reflexión (sin constructor público)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Muestra el valor predeterminado de IsVisible
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // Establece IsVisible a true
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // Establece IsVisible a false
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // Lee el valor actual de IsVisible
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // Guarda el libro de trabajo para demostrar una ejecución exitosa
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


