---
title: "Enum HtmlFormatHandlingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ExternalConnections.HtmlFormatHandlingType enum. Especifica cómo manejar el formato del origen HTML"
type: docs
url: /es/net/aspose.cells.externalconnections/htmlformathandlingtype/
---
## HtmlFormatHandlingType enumeration

Especifica cómo manejar el formato del origen HTML

```csharp
public enum HtmlFormatHandlingType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| All | `0` | Transferir todo el formato HTML a la hoja de cálculo junto con los datos. |
| None | `1` | Importar datos como texto sin formato (la configuración de tipos de datos aún ocurre). |
| Rtf | `2` | Traducir el formato HTML a formato de texto enriquecido en los datos importados a la hoja de cálculo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassHtmlFormatHandlingTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demostrar todos los valores de enumeración de HtmlFormatHandlingType
                HtmlFormatHandlingType allFormatting = HtmlFormatHandlingType.All;
                HtmlFormatHandlingType noFormatting = HtmlFormatHandlingType.None;
                HtmlFormatHandlingType rtfFormatting = HtmlFormatHandlingType.Rtf;

                // Mostrar los valores del enum
                Console.WriteLine("HtmlFormatHandlingType.All: " + allFormatting);
                Console.WriteLine("HtmlFormatHandlingType.None: " + noFormatting);
                Console.WriteLine("HtmlFormatHandlingType.Rtf: " + rtfFormatting);

                // Simular el uso de estos valores en un escenario
                worksheet.Cells["A1"].PutValue("Format Handling Types:");
                worksheet.Cells["A2"].PutValue("All Formatting");
                worksheet.Cells["A3"].PutValue("No Formatting");
                worksheet.Cells["A4"].PutValue("RTF Formatting");

                // Guarda el libro de trabajo
                workbook.Save("HtmlFormatHandlingTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in HtmlFormatHandlingType demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


