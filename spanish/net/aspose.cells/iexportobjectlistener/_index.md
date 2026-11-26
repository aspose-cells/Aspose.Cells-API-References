---
title: "Interfaz IExportObjectListener"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.IExportObjectListener. Permite a los usuarios manipular objetos durante la exportación"
type: docs
url: /es/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Permite a los usuarios manipular objetos durante la exportación.

```csharp
public interface IExportObjectListener
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Exporta un objeto. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassIExportObjectListenerDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añade una imagen de ejemplo a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Implementación personalizada del listener de exportación
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // Guarda como HTML con listener personalizado
            workbook.Save("output.html", saveOptions);
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        
        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                if (shape.MsoDrawingType == MsoDrawingType.Picture)
                {
                    string url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                    imgIdx++;
                    return url;
                }
            }
            return null;
        }
        
        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // En una implementación real, aquí guardarías la imagen en el disco
            // Para propósitos de demostración, solo devolvemos una ruta ficticia
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


