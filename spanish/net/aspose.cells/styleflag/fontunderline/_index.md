---
title: "StyleFlag.FontUnderline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración del subrayado de fuente"
type: docs
url: /es/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

Se aplicará la configuración de subrayado de fuente.

```csharp
public bool FontUnderline { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // Crear un objeto de estilo y establecer el subrayado de fuente
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // Crear una bandera de estilo y habilitar la bandera de subrayado de fuente
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // Aplicar el estilo a la celda con la bandera de estilo
            cell.SetStyle(style, styleFlag);

            // Mostrar el estado actual del subrayado
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Cambiar el tipo de subrayado a doble
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Guarda el libro de trabajo
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


