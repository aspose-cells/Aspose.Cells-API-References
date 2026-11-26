---
title: "WebQueryConnection.HtmlFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebQueryConnection. Cómo manejar el formato del origen HTML al traer datos de consulta web a la hoja de cálculo. Relevante cuando sourceData es True"
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

Cómo manejar el formato del origen HTML al incorporar datos de consulta web en la hoja de cálculo. Relevante cuando sourceData es True.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyHtmlFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera conexión de consulta web existente (si la hay)
            // O crear una nueva cargando un archivo con conexiones web
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // Mostrar el valor inicial de HtmlFormat
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Establecer HtmlFormat a Rtf (demostrando la operación de escritura)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Establecer HtmlFormat a None
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Guardar el libro con la conexión de consulta web
                    workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error: {ex.Message}");
                }
            }
            else
            {
                Console.WriteLine("No web query connections found in the workbook.");
            }
        }
    }
}
```

### Ver también

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


