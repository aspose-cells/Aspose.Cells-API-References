---
title: "Clase HeaderFooterCommand"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.HeaderFooterCommand. Representa el comando de encabezado/pie de página"
type: docs
url: /es/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Representa el comando de encabezado/pie de página

```csharp
public class HeaderFooterCommand
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Obtiene la fuente del valor del comando. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Obtiene el texto del comando. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Obtiene el tipo de comando de encabezado/pie de página. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a PageSetup y establezca el encabezado con comandos
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // Obtener comandos de encabezado
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // Mostrar tipos de comando y texto
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


