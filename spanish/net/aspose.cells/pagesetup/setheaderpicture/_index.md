---
title: "PageSetup.SetHeaderPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece una imagen en el encabezado de una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

Establece una imagen en el encabezado de una hoja de cálculo.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerPicture | Byte[] | Datos de imagen. |

### Valor de retorno

Devuelve el objeto [`Picture`](../../../aspose.cells.drawing/picture/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cargar un archivo de imagen en una matriz de bytes
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // Llamar a SetHeaderPicture con el índice de sección (0 para el encabezado central) y los bytes de la imagen
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // Establecer el script del encabezado para mostrar la imagen
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


