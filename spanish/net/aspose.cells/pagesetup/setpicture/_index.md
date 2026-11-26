---
title: "PageSetup.SetPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece una imagen en el encabezado/pie de página de una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

Establece una imagen en el encabezado/pie de página de una hoja de cálculo.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isFirst | Booleano | Indica si se está configurando la imagen del encabezado/pie de página de la primera página. |
| isEven | Booleano | Indica si se está configurando la imagen del encabezado/pie de página de una página par. |
| isHeader | Booleano | Indica si se está configurando la imagen del encabezado/pie de página. |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| imageData | Byte[] | Datos de imagen. |

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

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Cargar un archivo de imagen en una matriz de bytes
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // Llamar al método SetPicture para establecer la imagen del encabezado
                // Parámetros: isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // Establecer el texto del encabezado
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // Guarda el libro de trabajo
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
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


