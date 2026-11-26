---
title: "HeaderFooterCommand.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HeaderFooterCommand. Obtiene el texto del comando"
type: docs
url: /es/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Obtiene el texto del comando.

```csharp
public string Text { get; }
```

### Observaciones

Solo válido para HeaderFooterCommandType.Text.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer encabezado con comando de texto
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // Obtener comandos de encabezado
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // Mostrar información sobre el comando de texto
            foreach (HeaderFooterCommand cmd in commands)
            {
                if (cmd.Type == HeaderFooterCommandType.Text)
                {
                    Console.WriteLine("Text command found:");
                    Console.WriteLine("Text: " + cmd.Text);
                    Console.WriteLine("Font: " + cmd.Font);
                    Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
                }
            }
            
            // Guarda el libro de trabajo
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


