---
title: "Clase ExportObjectEvent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ExportObjectEvent. El evento se dispara al exportar un objeto como Picture"
type: docs
url: /es/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

El evento se dispara al exportar un objeto, como Picture.

```csharp
public class ExportObjectEvent
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Obtiene el objeto que será exportado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventDemo
    {
        public static void ExportObjectEventExample()
        {
            // Implementación personalizada de IExportObjectListener
            // Guarda el archivo HTML con un listener personalizado
            Workbook workbook = new Workbook(); // Build your workbook here
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = new CustomExportObjectListener()
            };
            using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
            {
                workbook.Save(stream, saveOptions); // Save the workbook to stream
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;

        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape shape)
            {
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                        break;
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }

        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // Aquí guarda la imagen en cualquier ubicación, luego devuelve la URL (relativa o absoluta) que el HTML generado puede usar para obtener la imagen
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


