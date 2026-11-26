---
title: "HeaderFooterCommand.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HeaderFooterCommand. Obtiene la fuente del valor del comando"
type: docs
url: /es/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

Obtiene la fuente del valor del comando.

```csharp
public Font Font { get; }
```

### Observaciones

Inútil para HeaderFooterCommandType.Picture.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la configuración de página para encabezado/pie de página
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer un encabezado con texto que tendrá un HeaderFooterCommand
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // Obtener script de encabezado
            string headerScript = pageSetup.GetHeader(0);

            // Obtener comandos de encabezado
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // Buscar el comando de texto (asumiendo que es el primero)
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // Acceder a la propiedad Font (solo lectura)
                Font font = textCommand.Font;
                
                // Mostrar propiedades actuales de la fuente
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // Dado que Font es solo lectura, no podemos asignar un nuevo objeto Font,
                // pero podemos modificar las propiedades de la fuente existente
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // Guarda el libro de trabajo para ver los cambios
                workbook.Save("HeaderFooterFontDemo.xlsx");

                Console.WriteLine("\nModified Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");
            }
        }
    }
}
```

### Ver también

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


