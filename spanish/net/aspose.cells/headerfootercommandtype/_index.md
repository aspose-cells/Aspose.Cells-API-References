---
title: "Enumeración HeaderFooterCommandType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.HeaderFooterCommandType. Representa el tipo de comando del encabezado y pie de página"
type: docs
url: /es/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Representa el tipo de comando de encabezado y pie de página.

```csharp
public enum HeaderFooterCommandType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Text | `0` | El texto. |
| CurrentPage | `1` | Número de página actual |
| Pagecount | `2` | Recuento de páginas |
| CurrentDate | `3` | Fecha actual |
| CurrentTime | `4` | Hora actual |
| SheetName | `5` | Nombre de la hoja |
| FileName | `6` | Nombre de archivo sin ruta |
| FilePath | `7` | Ruta del archivo sin nombre de archivo |
| Picture | `8` | Imagen |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Establecer encabezado con diferentes tipos de comando
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Recuperar comandos de encabezado
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Demostrar diferentes valores de HeaderFooterCommandType
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Comprobar tipos de comando específicos
                    if (cmd.Type == HeaderFooterCommandType.CurrentPage)
                    {
                        Console.WriteLine("Found CurrentPage command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.Pagecount)
                    {
                        Console.WriteLine("Found Pagecount command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentDate)
                    {
                        Console.WriteLine("Found CurrentDate command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentTime)
                    {
                        Console.WriteLine("Found CurrentTime command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.FileName)
                    {
                        Console.WriteLine("Found FileName command");
                    }
                }

                // Guardar el libro de trabajo para demostrar la configuración del encabezado
                workbook.Save("HeaderFooterCommandTypeDemo.xlsx");
                Console.WriteLine("HeaderFooterCommandType demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HeaderFooterCommandType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


