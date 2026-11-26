---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ConditionalFormattingIcon. Obtener los datos del conjunto de iconos"
type: docs
url: /es/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

Obtener los datos del conjunto de íconos

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | IconSetType | tipo del icono |
| índice | Int32 | índice del icono |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // No es necesario crear una instancia ya que GetIconImageData es estático
            
            try
            {
                // Llamar a GetIconImageData con IconSetType.Arrows3 e índice 0
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // Guardar los datos de la imagen en un archivo para demostración
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


