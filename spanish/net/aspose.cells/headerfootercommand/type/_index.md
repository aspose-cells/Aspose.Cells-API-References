---
title: "HeaderFooterCommand.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HeaderFooterCommand. Obtiene el tipo de comando de encabezado/pie de página"
type: docs
url: /es/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Obtiene el tipo de comando de encabezado/pie de página.

```csharp
public HeaderFooterCommandType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer encabezado con diferentes tipos de comando
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // Obtener comandos de encabezado
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### Ver también

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


