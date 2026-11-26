---
title: "PageSetup.GetPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene el objeto Picture del encabezado / pie de página"
type: docs
url: /es/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Obtiene el objeto [`Picture`](../../../aspose.cells.drawing/picture/) del encabezado / pie de página.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isHeader | Booleano | Indica si está en el encabezado o en el pie de página. |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

### Valor de retorno

Devuelve el objeto [`Picture`](../../../aspose.cells.drawing/picture/). Devuelve null si no hay imagen.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue una imagen al encabezado de la hoja de cálculo
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // Obtenga la imagen del encabezado y modifique su brillo
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Obtiene el objeto [`Picture`](../../../aspose.cells.drawing/picture/) del encabezado / pie de página.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isFirst | Booleano | Indica si se está obteniendo la imagen del encabezado/pie de página de la primera página. |
| isEven | Booleano | Indica si se está obteniendo la imagen del encabezado/pie de página de las páginas pares. |
| isHeader | Booleano | Indica si se está obteniendo la imagen del encabezado/pie de página. |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

### Valor de retorno

Devuelve el objeto [`Picture`](../../../aspose.cells.drawing/picture/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener el objeto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establezca algunas propiedades de encabezado/pie de página para asegurar que tengamos imágenes para recuperar
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // Llame al método GetPicture con los parámetros: isFirst, isEven, isHeader, section
                // Comprobando el encabezado de la primera página (sección 0 - encabezado central)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
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


