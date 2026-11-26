---
title: "PageSetup.GetCommands"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene todos los comandos del encabezado o pie de página"
type: docs
url: /es/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Obtiene todos los comandos del encabezado o pie de página.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| headerFooterScript | String | El script de encabezado/pie de página |

### Valor de retorno

Devuelve todos los comandos del encabezado o pie de página.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer encabezado con comandos
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // Obtener comandos de encabezado
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // Mostrar tipos de comando y texto
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### Ver también

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


