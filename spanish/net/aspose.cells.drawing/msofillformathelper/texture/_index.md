---
title: "MsoFillFormatHelper.Texture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFillFormatHelper. Obtiene el tipo de relleno de textura"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Obtiene el tipo de relleno de textura.

```csharp
public TextureType Texture { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una etiqueta para que el ejemplo sea significativo
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Crear una instancia de MsoFillFormatHelper usando reflexión (sin constructor público)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Mostrar el valor actual de la propiedad Texture (solo lectura)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Demostrar que la propiedad es solo lectura intentando establecerla (comentado)
                // fillHelper.Texture = TextureType.Canvas; // Esto causaría un error de compilación

                // Mostrar todos los tipos de textura disponibles como referencia
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Guarda el libro de trabajo para demostrar una ejecución exitosa
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


