---
title: "StyleFlag.TextDirection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "StyleFlag propiedad. La configuración de dirección de texto se aplicará"
type: docs
url: /es/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

Se aplicará la configuración de dirección de texto.

```csharp
public bool TextDirection { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // Crear un estilo y establecer la dirección de texto
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // Crear una bandera de estilo y habilitar la bandera TextDirection
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // Aplicar el estilo a la celda con la bandera de estilo
            cell.SetStyle(style, styleFlag);

            // Mostrar la dirección de texto actual
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Cambiar la dirección de texto y aplicar de nuevo
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Guarda el libro de trabajo
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


