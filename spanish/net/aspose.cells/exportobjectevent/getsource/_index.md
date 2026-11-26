---
title: "ExportObjectEvent.GetSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExportObjectEvent. Obtiene el objeto que se exportará"
type: docs
url: /es/net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Obtiene el objeto que será exportado.

```csharp
public object GetSource()
```

### Valor de retorno

el objeto que se exportará.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventMethodGetSourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen para demostrar la funcionalidad GetSource
            int pictureIndex = worksheet.Pictures.Add(1, 1, "sample.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            try
            {
                // Crear un listener de exportación de objetos personalizado
                HtmlSaveOptions saveOptions = new HtmlSaveOptions
                {
                    ExportObjectListener = new CustomExportObjectListener()
                };

                // Guardar el libro de trabajo para activar el ExportObjectEvent
                using (Stream stream = new FileStream("GetSourceDemo.html", FileMode.Create))
                {
                    workbook.Save(stream, saveOptions);
                }

                Console.WriteLine("GetSource method demonstrated successfully. Check the output HTML file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetSource: {ex.Message}");
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Demostrar el método GetSource
            object source = e.GetSource();

            if (source is Picture)
            {
                Console.WriteLine("GetSource returned a Picture object");
                return "custom-image-url.jpg";
            }

            return null;
        }
    }
}
```

### Ver también

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


