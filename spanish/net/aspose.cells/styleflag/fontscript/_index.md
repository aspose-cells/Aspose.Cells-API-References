---
title: "StyleFlag.FontScript"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración del script de fuente"
type: docs
url: /es/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

Se aplicará la configuración de script de fuente.

```csharp
public bool FontScript { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer algún texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Crear un objeto de estilo y establecer el script de fuente a subíndice
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // Crear una bandera de estilo y habilitar la bandera FontScript
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // Aplicar el estilo a la celda con la bandera de estilo
            cell.SetStyle(style, styleFlag);

            // Mostrar el estado actual del script de fuente
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Cambiar el script de fuente a superíndice
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // Mostrar el estado actualizado del script de fuente
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Guarda el libro de trabajo
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


