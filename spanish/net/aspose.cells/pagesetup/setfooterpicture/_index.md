---
title: "PageSetup.SetFooterPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece una imagen en el pie de página de una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

Establece una imagen en el pie de página de una hoja de cálculo.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| footerPicture | Byte[] | Datos de imagen. |

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

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cargar un archivo de imagen en una matriz de bytes
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // Llame al método SetFooterPicture con el índice de sección (0 para centro, 1 para izquierda, 2 para derecha) y los datos de la imagen
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // Establezca el texto del pie de página para que se muestre junto con la imagen
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // Guarde el libro de trabajo para ver la imagen del pie de página
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


